# Executable Files
## Code:
```bash
hacker@permissions~executable-files:~$ chmod o+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
ssh-entrypoint: /challenge/run: Permission denied
-r--r--r-x 1 hacker hacker 32 Jul  4 06:37 /challenge/run
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{YDvF6VGpIDkys-PbqRxuGbakqeX.dJTM2QDLycjN0czW}
```
## Learnings:
- In this challenge, I learned about execute permissions.
- I encountered a "Permission denied" error when trying to run `/challenge/run`. After realizing I needed to use `chmod u+x /challenge/run` for myself, I successfully executed the program and retrieved the flag.
## References:
None

