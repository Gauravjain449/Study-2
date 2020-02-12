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

sudo apt install default-jdk-headless
sudo apt-get install language-pack-en
wget -q -O - http://pkg.jenkins-ci.org/debian/jenkins-ci.org.key | sudo apt-key add -
echo "deb http://pkg.jenkins-ci.org/debian binary/" | sudo tee -a /etc/apt/sources.list.d/jenkins.list
sudo apt-get update
sudo apt-get install jenkins

verify jenkins by typing

ps -ef | grep jenkins

wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -.




