# Project 4

**Backend Configuration**
___

updating ubuntu

` $ sudo apt update`

![](images/update1.png)

upgrading ubuntu

`$ sudo apt upgrade`

![](images/upgrade2.png)

adding certificates

`$ sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates`

`$ curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`

![](images/certs3.png)

**installing nodejs**

`$ sudo apt install -y nodejs`

![](images/nodeinstall4.png)

**installing mongodb**

` $ sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6`

` $ echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list`

` $ sudo apt install -y mongodb`

![](images/mongoinstall5.png)

starting the server

` $ sudo service mongodb start`

` $ sudo systemctl status mongodb`

![](images/strtstatus6.png)

installing aptitude to download npm

` $ sudo apt install aptitude`

` $ sudo aptitude install npm`

![](images/instalaptitude7.png)

![](images/instalnpm8.png)

installing body-parser package to help process json files passed in requests to the server

` $ sudo npm install body-parser`

![](images/bodyparser9.png)

creating and entering the books directory

` $ mkdir books && cd books`

initializing npm project

` $ npm init`

creating and adding the server.js file to the directory

`vi server.js`

![](images/books&server10.png)

![](images/serverjs12.png)


**installing express and setting up the routes to the server**

installing mongoose and express

` $ sudo npm install express mongoose`

creating and entering the apps folder from the books folder

` $ mkdir apps && cd apps`

creating the routes.js file

` $ vi routes.js`

![](images/mongoose2routes12.png)

![](images/routes13.png)

creating the models folder from the apps directory

` $ mkdir models && cd models`

creating the book.js file

` $ vi book.js`

![](images/models2book14.png)


**accessing the routes with angularjs**

going back to books directory

` $ cd ../..`

creating the public directory

` $ mkdir public && cd public`

adding the script.js file

` $ vi script.js`

![](images/public2script15.png)

creating the index.html file in the public folder

` $ index.html`

![](images/index16.png)

going back to books directory

` $ cd ..`

starting the server with the following command:

` $ node server.js`

![](images/startingserver17.png)

curl testing on a different virtual machine to see what the command returns

` $ curl -s http://localhost:3000`

![](images/curltest18.png)

editing inbound rules to add tcp port 3300

![](images/inbound19.png)

getting public ip address

` $ curl -s http://169.254.169.254/latest/meta-data/public-ipv4`

![](images/ip20.png)

web book register application in the browser

![](images/final21.png)



