# apache-tomcat-setup
Apache Tomcat Setup Script


Update users information is the tomcat-users.xml file. 
#vi /opt/tomcat/conf/tomcat-users.xm and add the below user configuration at the last line of the file

<role rolename="manager-gui"/>
 <role rolename="manager-script"/>
 <role rolename="manager-jmx"/>
 <role rolename="manager-status"/>
 <user username="admin" password="admin" roles="manager-gui, manager-script, manager-jmx, manager-status"/>
 <user username="deployer" password="deployer" roles="manager-script"/>
 <user username="tomcat" password="s3cret" roles="manager-gui"/>


