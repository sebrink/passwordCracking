Finally we are going to be using a rule based attack. We will be replacing o's, e's, and a's with 0's, 3's, and @'s.

We will be attempting to break 2 passwords with this.

To view the files run the following:
	View the wordlist: `cat ./step4/wordlist.txt`{{execute}}

	View the hashes: `cat ./step4/hash.txt`{{execute}}

	View the rules: `cat ./john-local.conf`{{execute}}

To crack the passwords, run the following command:
	`john --format=raw-md5 --wordlist ./step4/wordlist.txt --rules=exampleRule ./step4/hash.txt`{{execute}}
