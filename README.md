# terraform-pipeline

setup steps

1) Jenkins installation

yum list java* - it will list java versions available

yum install java

--> Java install

sudo wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
sudo yum upgrade

# Add required dependencies for the jenkins package
sudo yum install fontconfig java-17-openjdk
sudo yum install jenkins
sudo systemctl daemon-reload

-----------------------------------------------
enable the Jenkins service to start at boot with the command:
--> sudo systemctl enable jenkins

start the Jenkins service with the command:
--> sudo systemctl start jenkins
terraform installation
--> 


