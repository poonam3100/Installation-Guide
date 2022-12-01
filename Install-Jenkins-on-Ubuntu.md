#Update system

sudo apt update


#Install java

sudo apt install openjdk-11-jre


#Validate Installation

java -version


#Run the following command

wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key |sudo gpg --dearmor -o /usr/share/keyrings/jenkins.gpg

sudo sh -c 'echo deb [signed-by=/usr/share/keyrings/jenkins.gpg] http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'

sudo apt update

sudo apt install jenkins

#check-jenkins installation setup

sudo systemctl status jenkins
