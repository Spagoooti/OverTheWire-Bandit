# Description
The credentials for the next level can be retrieved by submitting the password of the current level to **a port on localhost in the range 31000 to 32000**. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.
# Commands
ssh, telnet, nc, openssl, s_client, nmap
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit16 <br />
2.) Make a new directory under the "tmp" directory. <br />
3.) Change directory to the new directory you made. <br />
4.) Scan the network for open ports in the range 31000 to 32000. <br />
5.) Ssl into port 31790 and input the password of the current level. Copy the Rsa key. <br />
6.) Create a new file named "rsakey.private". <br />
7.) Open the file named "rsakey.private", paste the Rsa key, and save it to the file. <br />
8.) Change the permissions of "rsakey.private" to owner read-only. <br />
9.) Ssh into the Bandit server and log in as bandit17 using the Rsa key. <br />
10.) Open the file at "/etc/bandit_pass/bandit17" save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit16 <br />
2.) mkdir /tmp/directoryname <br />
3.) cd /tmp/directoryname <br />
4.) nmap -sV localhost -p 31000-32000 <br />
5.) ncat --ssl localhost 31790 <br />
6.) echo rsakey.private <br />
7.) nano rsakey.private <br />
8.) chmod 400 rsakey.private <br />
9.) ssh -i keyname.private bandit17@localhost -p 2220 <br />
10.) cat /etc/bandit_pass/bandit17
# Password
Bandit17: VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back]()