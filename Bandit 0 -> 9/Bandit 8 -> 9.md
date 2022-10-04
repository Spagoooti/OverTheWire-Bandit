# Description
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once.
# Commands
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit8 <br />
2.) Search "data.txt" for unique line and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit8 <br />
2.) sort data.txt | uniq -u
# Password
Bandit9: EN632PlfYiZbn3PhVK3XOGSlNInNE00t <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back]()
