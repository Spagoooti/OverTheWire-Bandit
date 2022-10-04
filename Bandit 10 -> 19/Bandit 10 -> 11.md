# Description
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data.
# Commands
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit10 <br />
2.) Decrypt the base64 encoded data within "data.txt" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit10 <br />
2.) base64 -d data.txt
# Password
Bandit11: 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back]()
