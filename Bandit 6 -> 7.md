# Description
The password for the next level is stored somewhere on the server and has all of the following properties: <br /> <br />
owned by user bandit7 <br />
owned by group bandit6 <br />
33 bytes in size
# Commands
ls, cd, cat, file, du, find
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit6. <br />
2.) Change directory to the root directory. <br />
3.) Search subdirectories for a file with the above qualities. <br />
4.) Open the file that does not return "permission denied" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit6 <br />
2.) cd / <br />
3.) ls -la <br />
4.) find . -user bandit7 -group bandit6 -size 33c <br />
5.) cat ./var/lib/dpkg/info/bandit7.password
# Password
Bandit7: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%202%20-%3E%203.md)
