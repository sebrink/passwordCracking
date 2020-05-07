Next we are going to be cracking 10 passwords with mask attacks. The masks we will be using are a year with a special character on the end (i.e. 2020!)

We will be appending this mask to the name of my dog, Wally.

To view the files run the following:

	View my dog's name: `cat ./step3/wally.txt`{{execute}}

	View the hashes: `cat ./step3/hash.txt`{{execute}}

To crack the passwords, run the following command:

	`john --format=Raw-md5 -w=./step3/wally.txt -mask=?w?d?d?d?d?s ./step3/hash.txt`{{execute}}
