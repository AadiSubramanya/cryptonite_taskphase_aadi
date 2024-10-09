# Duplicating piped data with tee
## Code:
```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee error.log | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat error.log
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "A6dJ9c-g"

hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret A6dJ9c-g | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{A6dJ9c-gNx_bWg0drwEeIwi9jjf.dFjM5QDLycjN0czW}
```
## Learnings:


## References:
none


