         Below are the details of the test. The test is divided into 6 steps, beginning with setting up the infrastructure to installing software and configuring the servers. Our preferred infrastructure automation tools are Terraform and Ansible, but it’s not mandatory to use them. Feel free to use the tools of your choice.  

Create two EC2 Instances in AWS Cloud using,
               Additional Information
Instance Type of both instance is t2.micro
Operating System for both instances Ubuntu Server 16.04 LTS
Hostname of Instance 1 : MSR-test-Instance-1
Hostname of Instance 2 : MSR-test-Instance-2
ssh -i "ubuntu.pem" ubuntu@ec2-13-234-94-225.ap-south-1.compute.amazonaws.com

ssh -i "ubuntu.pem" ubuntu@ec2-13-232-126-190.ap-south-1.compute.amazonaws.com

              Preferred tools but not mandatory – Terraform

Once these two servers are provisioned, ensure the below following software packages are installed using configuration management tool in both the provisioned instances.

Installed in Servers with help of apt install
NVM – Version 0.33.2
Node – 8.12.0
Docker – 18.06 or latest
Docker Compose – 1.13 or latest
Openssl – latest version
Git – latest version
          
Create a Docker Container in MSR-test-Instance-1 using Docker Compose file and ensure apache webserver is installed. Try to use configuration management tools to automate the entire installation of apache and deploy a sample html file from a GitHub repository.
             Additional Information
You can create your own GitHub repository with a sample html file.
http://13.234.94.225:4000/
http://13.232.126.190:4000/

             
Create a Docker Container in MSR-test-Instance-2 using Docker Compose file and ensure CouchDB Database is installed. Try to use any configuration management tool to automate the entire installation processes.
http://13.234.94.225:8080/
User name:- passwd:-2v4PcVP(gWYa30tQtB

http://13.234.94.225:4000/
http://13.232.126.190:8080/
User name Veerakumar  Passwd :-Astro1234
http://13.232.126.190:4000/

            Additional Information

We should be able to access the Futon – web GUI of CouchDB, from the external system.
        Git Repo :- git@github.com:veerakumarmail/test.git
Commit all the code/files to GitHub and write your explanations and documentations into the readme.
It will be an added advantage if you can draft the step by step procedure in performing the above activities and how to execute the code.

