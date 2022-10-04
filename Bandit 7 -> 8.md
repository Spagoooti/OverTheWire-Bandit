# Description
The password for the next level is stored in the file **data.txt** next to the word **millionth**.
# Commands
man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit7 <br />
2.) Search "data.txt" for a line containing the term "millionth".
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit7<br />
2.) grep "millionth" data.txt
# Password
Bandit8 TESKZC0XvTetK0S9xNwm25STk5iWrBvP <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%206%20-%3E%207.md)
