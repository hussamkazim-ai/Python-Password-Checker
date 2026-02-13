# Python-Password-Checker
A terminal-based tool to check how many times a password has been pwned using Python.

Command to run this script: python main.py yourpasswordhere

Here's how it works:

1: We convert the password that we want to check to SHA1 encoding
2: We send the 1st 5 characters of the SHA1 encoded password to pwnedpasswords.com
3: Pwnedpasswords.com returns a list of the pwned passwords' hashes that start with the same 1st 5 characters that we have sent to pwnedpasswords.com, along with how many times a hashed password has been pwned
4: We match the tails of hashes that came from pwnedpasswords.com with our hashed password's tail
5: If we find a match, we will get the number of how many times our password has been pwned in the terminal
6: If the password hash hasn't matched any of the hashes that came from pwnedpasswords.com, then we will get a message in the terminal that you should continue with that password
