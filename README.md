# ONOS-Docker
The ONOS controller is pre-installed to be used as an image file for Docker.

OS: Ubuntu:latest Docker image

ONOS: 2.4.0

---------------------------------------------------------------------------------------------------------------------

Download the file from:
https://drive.google.com/file/d/1520O9pPML2keTY6wz6v7YdecmafUT7j9/view?usp=sharing

---------------------------------------------------------------------------------------------------------------------
Execute the following commands in Windows CMD running Docker Desktop:

docker import C:\users\Billy\Desktop\ONOS.tar onos

docker run -it -p 8181:8181 -p 8101:8101 -p 9876:9876 -p 6653:6653 -p 6640:6640 --entrypoint "/bin/bash" onos

---------------------------------------------------------------------------------------------------------------------
Note: Prior to start up of ONOS make sure your $JAVA_HOME and $PATH variables are set with the 'export' function

export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64

export PATH=$PATH:$JAVA_HOME/bin
