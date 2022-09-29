# Description
The password for the next level is stored in a file called **spaces in this filename** located in the home directory.
# Commands
ls, cd, cat, file, du, find
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit2. <br />
2.) Search the home directory for a file called "spaces in this filename". <br />
3.) Open the file named "spaces in this filename" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 bandit2 <br />
2.) ls -la <br />
3.) cat "spaces in this filename"
# Password
Bandit3: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md)
