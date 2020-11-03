# redhat-wso2-api-manager-rpm-installation

RPM Package Installation : 

Get it - 

Site address - Download page : https://wso2.com/api-management/

Site address - Documentation page : https://apim.docs.wso2.com/en/latest/

Downlaod package and copy to below ,

[root@localhost 3.2.0]# pwd

/usr/lib64/APIManager/3.2.0

[root@localhost 3.2.0]# ls -ltr


Install it -

[root@localhost 3.2.0]# rpm -ivh wso2am-linux-installer-x64-3.2.0.rpm

WSO2 API Manager Installed on : "/usr/lib64/wso2/wso2am/3.2.0/"

To update WSO2 API Manager as a service, open a new terminal and run:
$ sudo -u wso2 /usr/lib64/wso2/wso2am/3.2.0/bin/update_linux

To run WSO2 API Manager as a service, open a new terminal and run:
$ sudo service wso2am-3.2.0 start

[root@localhost 3.2.0]# sudo service wso2am-3.2.0 start


Controll it - 

Running the Product

Starting the server

To start the server, <PRODUCT_HOME>/bin/wso2server.sh which is "/usr/lib64/wso2/wso2am/3.2.0/bin" 

To start the server in the background mode of Linux: sh wso2server.sh start To stop the server running in this mode, you will enter: sh wso2server.sh stop

Configuration file : /usr/lib64/wso2/wso2am/3.2.0/repository/conf


Access it  -

Publisher - https://localhost:9443/publisher

Store - https://localhost:9443/devportal

Admin console - https://localhost:9443/admin

Carbon console - https://localhost:9443/carbon


Uninstall - 

[root@localhost ~]# rpm -qa | grep -i "wso2"

[root@localhost ~]# rpm -e wso2am-3.2.0-1.el7.x86_64
