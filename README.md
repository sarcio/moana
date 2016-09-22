# moana
Monitor and Alarm

## Require

  * JRE (Java Runtime Enviroment) 1.6+ 
  * HTTP Port for Embedded Jetty Server


## Usage

  $ java -jar moana.jar -s -i [IP] -p [Port]
  
  * IP : Listen IP address for Embedded Jetty Web Server
  * Port : Listen port for Embedded Jetty Web Server
  
  
## Configure

  * conf/moana.conf
  * conf/list.conf
 

## List format (list.conf)

    type:IP:Port:URI:Name

e.g. 

    was:192.168.1.101:8080:/jmon/:TOMCAT_1
    was:192.168.1.102:8080:/jmon/:TOMCAT_2
    httpd:192.168.2.101:80:/server-status:HTTPD_1
    httpd:192.168.2.102:80:/server-status:HTTPD_2
    url:hr.moana.sarc.io.test:80:/hr/login.do:MOANA_HR_LOGIN
    url:crm.moana.sarc.io.test:80:/crm/login.do:MOANA_CRM_LOGIN
