# AmazonLinux2VaporServerConfigs
### Purpose
Commands and configs to get an Amazon Linux 2 server up and running with Vapor 4, Nginx 1.20.0, Swift 5.5.1, and systemd. These aren't shell scripts, at some point they will be, but at the moment they are disperate commands and config files. Some commands may need to be changed slightly, but this is how I got a Vapor 4 server up and running on Amazon Linux 2. A lot of tutorials I have seen use a program called Supervisor, but I figured out how to accomplish the same thing with systemd (it runs the vapor server, and restarts it if it goes down). From what I have read, Supervisor comes in handy when you are using containers, if you are using docker, that may be the way to go.
### Requirements
An AWS EC2 (Elastic Compute Cloud) Account<br>
An AMI instance with minimum type of t2.micro (I had to add a swap file of 2GB on my t2 to get Vapor to build, it will fail without)  
