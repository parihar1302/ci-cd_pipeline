# ci-cd_pipeline
This project consiste CICD Jenkins pipeline 
-----------------------------------------------

Step-1.) Launch a EC2 instance (Amazon Linux2 22.04)

## Note:- Open Custome TCP Port 8080 because Jenkins run on it



Step-2.) Install Jenkins packages/dependency
$ sudo wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
$ sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
$ sudo yum upgrade


## Now Installaing Javwa because jenkins runtime is Java only. Without java, jenkins will not run.
$ sudo yum -y install java-17*


## Now Installing Jenkins
$ sudo yum -y install jenkins

## Now reload & restart Jenkins
$ sudo systemctl daemon-reload
$ sudo systemctl start Jenkins
$ sudo systemctl enable Jenkins
$ sudo systemctl status Jenkins
----------------------------------------------------------------------
