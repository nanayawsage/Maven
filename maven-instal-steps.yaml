Maven Installation Steps on Ubuntu:
NB: t2.micro ec2 instance

# Changing The Hostname of The EC2 
sudo hostnamectl set-hostname maven
sudo su - ubuntu

# Update and Upgrade the Ubuntu EC2
sudo apt update -y
sudo apt upgrade -y

# Installation of Java and Git
cd /opt
sudo apt install default-jdk git -y

# Verify The Installation Of Java and Git
java -version
git --version

# Installing and Extracting Apache Maven
sudo wget https://dlcdn.apache.org/maven/maven-3/3.9.6/binaries/apache-maven-3.9.6-bin.tar.gz
sudo tar -xvzf apache-maven-3.9.6-bin.tar.gz

# Remove The Zip File and Rename the Extracted File
sudo rm -rf apache-maven-3.9.6-bin.tar.gz
sudo mv apache-maven-3.9.6/ maven

# Setting Up Environmental Variables for Maven
sudo vi ~/.bashrc
export M2_HOME=/opt/maven
export PATH=$PATH:$M2_HOME/bin

# Restart the .bashrc file
source ~/.bashrc

# Check The Installation Of Maven
mvn -version

NB: cd from the /opt directory after the Installation

# Make a directory named webapp-project
mkdir webapp-project
cd webapp-project

NB: the cloning must be done in the webapp-project directory you created

# Git clone the project repo
git clone https://github.com/JOMACS-IT/web-app.git

After cloning, you must change directory (cd) into the web-app directory before you start
executing any maven (mvn) goal