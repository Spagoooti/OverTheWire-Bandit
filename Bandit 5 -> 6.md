# Description
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties: <br /> <br />
human-readable <br />
1033 bytes in size <br />
not executable
# Commands
ls, cd, cat, file, du, find
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit5. <br />
2.) Search the home directory for a directory called "inhere". <br />
3.) Change from the home directory to the "inhere" directory. <br />
4.) Search subdirectories for a file with the above qualities. <br />
5.) Open the file named ".file2" under the "maybehere07" directory and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit5 <br />
2.) ls -la <br />
3.) cd inhere <br />
4.) ls -la <br />
5.) find . -type f -size 1033c ! -executable <br />
6.) cat ./maybehere07/.file2
# Password
Bandit6: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%204%20-%3E%205.md) [Next](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%206%20-%3E%207.md)
