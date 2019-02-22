# TomcatInit
### Tomcat自启动脚本

**How to use?**

- 设置tomcat自启动脚本：

  下载脚本：
  
  `wget https://github.com/wuhengzhen/TomcatInit/raw/master/init.d/Tomcat-init`
  
  `mv Tomcat-init /etc/init.d/tomcat`
  
- 添加执行权限：
  `chmod +x /etc/init.d/tomcat`
  
- 设置启动脚本JAVA_HOME：

  `sed -i 's@^export JAVA_HOME=.*@export JAVA_HOME=/usr/java/jdk1.8.0_191@' /etc/init.d/tomcat`
  
- 设置自启动：
  `chkconfig --add tomcat`
  
  `chkconfig tomcat on`
  
- 启动Tomcat：

  `service tomcat start`
  
