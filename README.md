# AmazonLinux2ServerSetup
### Purpose
Commands and configs to get an Amazon Linux 2 server up and running with Vapor 4, Nginx 1.20.0, Swift 5.5.1, and systemd. These aren't shell scripts, at some point they will be, but at the moment they are disperate commands that accomplish a goal. Some commands may need to be changed slightly, but these files are the basic way to get a Vapor 4 server up and running on Amazon Linux 2. A lot of tutorials I have seen use a program called Supervisor, but once I realized Supervisor was essentially just a python script, I decided to bag it because it was probably just using systemd under the hood. Also, Amazon Linux 2 doesn't have a yum install for Supervisor and the only way to install is using an outdated version of pip. Anyway, I felt like using Supervisor was a pain, so I figured out how to accomplish the same thing with systemd (it runs the vapor server, and restarts it if it goes down).
### Requirements
AWS EC2 (Elastic Compute Cloud) Account
AMI instance with minimum type of t2.micro (I had to add a swap file of 2GB on my t2 to get Vapor to build, it will fail without)  
