# /etc/profile
```
#tomcat1
export CATALINA_HOME=/root/Tools/apache-tomcat-9.0.22
export CATALINA_BASE=/root/Tools/apache-tomcat-9.0.22
export TOMCAT_HOME=/root/Tools/apache-tomcat-9.0.22

#tomcat2
export CATALINA_HOME2=/root/Tools/apache-tomcat-9.0.29
export CATALINA_BASE2=/root/Tools/apache-tomcat-9.0.29
export TOMCAT_HOME2=/root/Tools/apache-tomcat-9.0.29
```
#修改端口

直接修改server.xml文件

#修改start.sh文件，加入以下代码
```
export JAVA_HOME=/usr/local/jdk1.8.0_221
export PATH=$PATH:$JAVA_HOME/bin
export CLASSPATH=$JAVA_HOME/bin
export CATALINA_HOME=$CATALINA_HOME2
export CATALINA_BASE=$CATALINA_BASE2
```
#修改catalina.sh文件，加入一下代码
```
export CATALINA_BASE=$CATALINA_BASE2
export CATALINA_HOME=$CATALINA_HOME2
export TOMCAT_HOME=TOMCAT_HOME2
```
#最后分别启动两个tomcat
```
./start.sh
