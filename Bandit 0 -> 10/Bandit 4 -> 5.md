# Description
The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the “reset” command.
# Commands
ls, cd, cat, file, du, find
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit4. <br />
2.) Change from the home directory to the "inhere" directory. <br />
3.) Search  for a file within the folder that is human readable. <br />
4.) Open the file named "-file07" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit4 <br />
2.) cd inhere <br />
3.) file ./* <br />
4.) cat ./-file07
# Password
Bandit5: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%203%20-%3E%204.md) [Next](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%205%20-%3E%206.md)
