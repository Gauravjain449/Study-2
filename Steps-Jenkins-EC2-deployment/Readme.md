 chmod 600 /home/gauravjain449/Study-Phase-2/Private/AWS-Key/Home.pem
 ssh -i /home/gauravjain449/Study-Phase-2/Private/AWS-Key/Home.pem ubuntu@ec2-15-206-94-193.ap-south-1.compute.amazonaws.com

 chmod 600 /home/gauravjain449/Study-Phase-2/Private/AWS-Key/Home.pem

--------------
cat ~/.ssh/config
Host ec2
	Hostname 	ec2-15-206-94-193.ap-south-1.compute.amazonaws.com
	User 		ubuntu
	IdentityFile 	~/.ssh/Home.pem
-------------
mv /home/gauravjain449/Study-Phase-2/Private/AWS-Key/Home.pem ~/.ssh

-------------
https://gist.github.com/jsuwo/9038610
https://www.techrepublic.com/article/how-to-install-jenkins-on-ubuntu-server-18-04/

sudo apt install default-jdk-headless
sudo apt-get install language-pack-en
wget -q -O - http://pkg.jenkins-ci.org/debian/jenkins-ci.org.key | sudo apt-key add -
echo "deb http://pkg.jenkins-ci.org/debian binary/" | sudo tee -a /etc/apt/sources.list.d/jenkins.list
sudo apt-get update
sudo apt-get install jenkins

verify jenkins by typing

ps -ef | grep jenkins

sudo apt-get install apache2
sudo a2enmod proxy
sudo a2enmod proxy_http






