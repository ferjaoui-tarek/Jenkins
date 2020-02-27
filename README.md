# Jenkin

Jenkins Installation

Create an instance EC2 (linux)

ssh into your EC2 instance 

Update your system
```
sudo yum update
```

check your java version 
```
java -version
```

if you have many version installed you can choose aversion to check and select one out of multiple java versions available
```
sudo /usr/sbin/alternatives --config java
```

Install Java
```
 sudo yum install -y java-1.8.0-openjdk-devel
```

Install wget.
```
sudo yum install -y wget
```

Download the repo.
```
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo
```

Import the required key.
```
sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
```

Install Jenkins.
```
sudo yum install -y jenkins
```

