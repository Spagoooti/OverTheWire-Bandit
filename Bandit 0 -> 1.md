# Description
The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.
# Commands
ls, cd, cat, file, du, find
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit0 using the password bandit0.\n
2.) Search the home directory for a file called readme.\n
3.) Open the file named readme and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 bandit0\n
2.) ls -la\n
3.) cat readme\n
# Password
Bandit1: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
