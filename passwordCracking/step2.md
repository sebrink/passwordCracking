The first the we are going to be doing is cracking a 4 digit pin with a brute force attack.

We will be guessing every number from 0000 to 9999 in order to crack these passwords.

To view the files run the following:
	View the pins: `cat ./step1/10k-passwords.txt`{{execute}}

	View the hashes: `cat ./step1/10-hashes.txt`{{execute}}

To crack the passwords, run the following command:
	`john --format=raw-md5 --wordlist=./step1/10k-passwords.txt ./step1/10-hashes.txt`{{execute}}
