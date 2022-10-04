# Description
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)
# Commands
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file
# Walkthrough
1.) Ssh into the Bandit server and log in as bandit12 <br />
2.) Make a new directory under the "tmp" directory. <br />
3.) Copy "data.txt" from the home directory to the new directory you made. <br />
4.) Change directory to the new directory you made. <br />
5.) Reverse the hexdump named "data.txt". <br />
6.) Check the file type of "data". <br />
7.) Rename "data" to "data2.gz". <br />
8.) Decompress the gzip archive named "data2.gz". <br />
9.) Check the file type of "data2". <br />
10.) Rename "data2" to "data2.bzip2". <br />
11.) Decompress the bzip2 archive named "data2.bzip2". <br />
12.) Check the file type of "data2.bzip2.out". <br />
13.) Rename "data2.bzip2.out" to "data4.tar". <br />
14.) Decompress the tar archive named "data4.tar". <br />
15.) Check the file type of "data5.bin". <br />
16.) Rename "data5.bin" to "data5.tar". <br />
17.) Decompress the tar archive named "data5.tar". <br />
18.) Check the file type of "data6.bin". <br />
19.) Rename "data6.bin" to "data6.bzip2". <br />
20.) Decompress the bzip2 archive named "data6.bzip2". <br />
21.) Check the file type of "data6.bzip2.out". <br />
22.) Rename "data6.bzip2.out" to "data6.tar". <br />
23.) Decompress the tar archive named "data6.tar". <br />
24.) Check the file type of "data8.bin". <br />
25.) Rename "data8.bin" to "data8.gz". <br />
26.) Decompress the gzip archive named "data8.gz". <br />
27.) Open the file named "data8" and save the password.
# Solution
1.) ssh bandit.labs.overthewire.org -p 2220 -l bandit12 <br />
2.) mkdir /tmp/directoryname <br />
3.) cp data.txt /tmp/directoryname <br />
4.) cd /tmp/directoryname <br />
5.) xxd -r data.txt data <br />
6.) file data <br />
7.) mv data data2.gz <br />
8.) gzip -d data2.gz <br />
9.) file data2 <br />
10.) mv data2 data2.bzip2 <br />
11.) bzip2 -d data2.bzip2 <br />
12.) file data2.bzip2.out <br />
13.) mv data2.bzip2.out data4.tar <br />
14.) tar -xvf data4.tar <br />
15.) file data5.bin <br />
16.) mv data5.bin data5.tar <br />
17.) tar -xvf data5.tar <br />
18.) file data6.bin <br />
19.) mv data6.bin data6.bzip2 <br />
20.) bzip2 -d data6.bzip2 <br />
21.) file data6.bzip2.out <br />
22.) mv data6.bzip2.out data6.tar <br />
23.) tar -xvf data6.tar <br />
24.) file data8.bin <br />
25.) mv data8.bin data8.gz <br />
26.) gzip -d data8.gz <br />
27.) cat data8
# Password
Bandit13: wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw <br /> <br />
[Home](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/README.md) [Back](https://github.com/Spagoooti/OverTheWire-Bandit/blob/main/Bandit%2010%20-%3E%2019/Bandit%2011%20-%3E%2012.md)
