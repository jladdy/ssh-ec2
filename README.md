Description
===========

Allows users to ssh to EC2 instance by the either 8 or 17 character Instance ID.

Requirements
============

Tested with ec2-api-tools-1.7.5.1 


Configuration
=====

* Install EC2 Command Line Tools, instructions can be found [here](http://docs.aws.amazon.com/AWSEC2/latest/CommandLineReference/set-up-ec2-cli-linux.html#setting_up_ec2_command_linux).
* Place the ssh-ec2 script in somewhere in your environment path or add the desired location to your path and ensure it is executable.
* Place the ec2.vars file in your desired location, for this readme we will use the users home dir. 
* Configure the ec2.vars with your AWS Access ID, AWS Key ID, and the region in which your instances reside. 


Usage
=====

In order to use this tool you must first source your ec2.vars file. 

`. ~/ec2.vars`

If you have servers in multiple regions or multiple AWS account, you can create multiple .vars files. If not it may be easier to place these variables in your .bashrc. 

After that you can ssh to your instance ID with:

`ssh-ec2 i-xxxxxx`
