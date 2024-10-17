# Redirecting Script Output
## Code:
```bash
hacker@chaining~redirecting-script-output:~$ touch x.sh
hacker@chaining~redirecting-script-output:~$ echo "/challenge/pwn" >> x.sh
hacker@chaining~redirecting-script-output:~$ echo "/challenge/college" >> x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{cs0E2fXyXAre1Qifnb5HAC30Mak.dhTM5QDLycjN0czW}
```
## Learnings:
- Creating a script that runs multiple commands and redirect its output using piping.
## References:
None

