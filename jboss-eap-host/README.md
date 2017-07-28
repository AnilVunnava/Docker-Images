# Docker-Images

**This is a sample development/evaluation image for jboss-eap Host Controller.**

Thanks to _[fcarrus/jboss-eap-6.4-host] (https://hub.docker.com/r/fcarrus/jboss-eap-6.4-host/)_ Where in I had used the base as jboss-eap-6.4-host- and constructed a generic JBoss EAP Host Controller Image

## Creating JBoss EAP HostController Image.
1. git clone https://github.com/AnilVunnava/Docker-Images.git
2. navigate to folder jboss-eap-host
3. modify environment variables to .env file
  * JBOSS_HOST_NAME
  * JBOSS_DOMAIN_ADDRESS
  * JBOSS_DOMAIN_USERNAME
  * JBOSS_DOMAIN_SECRET
4. run command docker-compose up 
