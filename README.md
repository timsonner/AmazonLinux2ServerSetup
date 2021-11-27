# AmazonLinux2ServerSetup
### Purpose
Commands and configs to get an Amazon Linux 2 server up and running with Vapor 4, Nginx 1.20.0, Swift 5.5.1, and systemd. These aren't shell scripts, at some point they will be, but at the moment they are disperate commands that accomplish a goal. Some commands may need to be changed slightly, but these files are the basic way to get a Vapor 4 server up and running on Amazon Linux 2. Just follow the commands in the files, some echo commands may need to be pasted into the config files instead of "echoed."
### Requirements
AWS EC2 (Elastic Compute Cloud) Account
AMI instance with minimum type of t2.micro (I had to add a swap file of 2GB on my t2 to get Vapor to build, it will fail without)  
