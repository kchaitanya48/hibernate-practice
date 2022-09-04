Devops - Steps
-------------------------

Jenkins
--------

step1 : create EC2 environment and connect  
step2  : download jenkins software follwed by Jenkins Redhat-centos steps  
step3 : by Aws command amazon-linux-extras, install install java-openjdk11  --> amazon-linux-extras install java-openjdk11   
step 4: yum install git -y  
step 5: Install git plugin without restart Manage Jenkins > Jenkins Plugins > available > github 
step 6: Configure git path Manage Jenkins > Global Tool Configuration > git  
step 7 :create folder : mkdir /opt/maven   --->  cd /opt/maven  ---->    
step 8 : wget http://mirrors.estointernet.in/apache/maven/maven-3/3.6.1/binaries/apache-maven-3.6.1-bin.tar.gz
          tar -xvzf apache-maven-3.6.1-bin.tar.gz   
step 9 : vi ~/.bash_profile  
        M2_HOME=/opt/maven/apache-maven-3.6.1 
        M2=$M2_HOME/bin  
         PATH=<Existing_PATH>:$M2_HOME:$M2  
step 10 : Setup JAVA_HOME at ~/.bash_profile       
          find java path (find / -name jvm) 
	
         
DOCKER
-------------


docker build -t myimage . 

docker run -d --name myimage-container -p 8081:8778 myimage

docker exec -it tomcat-container  /bin/bash 

docker stop tomcat-container

docker rm container-id

docker rmi image-id

docker ps -a

docker images 

docker ps 


CREATE DOCKER ENVIORNMENT LINUX
---------------------------------


cat  /etc/passwd --> gives the user details 

cat /etc/groups   --> gives the group details 

useradd dockeradmin   --> adding new user - dockeradmin  

passwd dockeradmin    -> adding password for dockeradmin  

vi /etc/ssh/ssh_config  -> find password key by using /password at right corner of vi and enable password mode  

services sshd reload   --> reload or restart the services  





