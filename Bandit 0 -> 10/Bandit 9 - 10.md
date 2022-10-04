# Description
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.
# Commands
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit9 <br />
2.) Search "data.txt" for a human-readable string with several "=" characters and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit9 <br />
2.) strings data.txt | grep "===="
# Password
Bandit10: G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back]()