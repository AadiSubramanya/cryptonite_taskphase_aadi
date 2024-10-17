# Your First Shell Script
## Code:
```bash
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ echo "/challenge/pwn" >> x.sh
hacker@chaining~your-first-shell-script:~$ echo "/challenge/college" >> x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{MMeDRxVZEz4UrUmgvQ8Zo79QJmA.dFzN4QDLycjN0czW}
```
## Learnings:
- I created a shell script called `x.sh` to run the commands `/challenge/pwn` and `/challenge/college`. Using `echo` with quotes ensured the commands were stored correctly.
- Took me some time to realize that I had to use quotes in the echo commands to ensure that the entire command string was treated as a single argument (Without quotes, the shell could interpret parts of the command).
- Running `bash x.sh` executed both commands successfully.
## References:
None

