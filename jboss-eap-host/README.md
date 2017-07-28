# Docker-Images

**This is a sample development/evaluation image for jboss-eap Host Controller.**

Thanks to _[fcarrus/jboss-eap-6.4-host] (https://hub.docker.com/r/fcarrus/jboss-eap-6.4-host/)_ Where in I had used the base as jboss-eap-6.4-host- and constructed a generic JBoss EAP Host Controller Image

## Creating JBoss EAP HostController Image.
1. git clone https://github.com/AnilVunnava/Docker-Images.git
2. modify environment variables to .env file
    * JBOSS_DOMAIN_ADDRESS
    * JBOSS_DOMAIN_PORT
    * JBOSS_DOMAIN_USERNAME
3. modify the below in jboss-eap-host/host.xml
    * tag host name="**_slave_**" xmlns="urn:jboss:domain:1.7" name of host your host name and is unique for each host controller
    * tag secret value="**_xxxxxxx_**"/ to your domain controller's secret key value under tag security-realm name="ManagementRealm"
4. run command docker-compose up 
