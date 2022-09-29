# Description
The password for the next level is stored in a hidden file in the **inhere** directory.
# Commands
ls, cd, cat, file, du, find
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit3. <br />
2.) Search the home directory for a directory called "inhere". <br />
3.) Change from the home directory to the "inhere" directory. <br />
4.) Open the file names ".hidden" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 bandit3 <br />
2.) ls -la <br />
3.) cd inhere <br />
4.) ls -la <br />
5.) cat .hidden
# Password
Bandit4: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%202%20-%3E%203.md)
