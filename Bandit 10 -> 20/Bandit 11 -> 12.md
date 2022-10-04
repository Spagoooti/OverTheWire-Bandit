# Description
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions.
# Commands
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit11 <br />
2.) Decrypt the rot-13 encoded data within "data.txt" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit11 <br />
2.) cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
# Password
Bandit12: JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%2010%20-%3E%2020/Bandit%2010%20-%3E%2011.md) [Next](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%2010%20-%3E%2020/Bandit%2012%20-%3E%2013.md)
