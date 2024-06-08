Steps and commands - 

AWS EC2 config for nodejs app

1-Create  EC2 instance with ubuntu running 

2- Connect to your Ubuntu instance 

3-Once you have your Ec2 Ubuntu command line access run the system update command to ensure all the 

existing packages are up to date.

sudo apt update

4-check if Nodejs is installed or not 

sudo apt policy nodejs

5-Add Nodejs  LTS repo on Ec2 Ubuntu

curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -

6-Install Nodejs and NPM
sudo apt-get install nodejs

7- See  the version

node -v

npm -v

8-install pm2 globally

npm i pm2 -g 
9-install and setup git

sudo apt install git

git —version

git config --global user.name "Your Name"

git config --global user.email "youremail@domain.com"

git config --list

10- Clone your GitHub repo of your project o transfer codes through FileZilla  or through scp command

Git clone “githubrepo.url”

11- Run your code with            
npm install

Pm2 start index.js