Next we are going to be cracking 10 passwords with a dictonary based attack. The wordlist we are using is the top 10,000 worst passwords.

We will be looping through our list of 10,000 words in order to guess the password.

To view the files run the following:
	- View the wordlist: `cat ./step2/10k-common.txt`{{execute}}
	- View the hashes: `cat ./step2/passwords.txt`{{execute}}

To crack the passwords, run the following command:
	- `john --format=raw-md5 --wordlist=./step2/10k-common.txt ./step2/passwords.txt`{{execute}}
