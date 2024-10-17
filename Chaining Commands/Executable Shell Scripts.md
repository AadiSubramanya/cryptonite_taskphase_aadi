# Executable Shell Scripts
## Code:
```bash
hacker@chaining~executable-shell-scripts:~$ touch script.sh
hacker@chaining~executable-shell-scripts:~$ echo "/challenge/solve" >> script.sh
hacker@chaining~executable-shell-scripts:~$ ls -l script.sh
-rw-r--r-- 1 hacker hacker 17 Oct 17 18:11 script.sh
hacker@chaining~executable-shell-scripts:~$ chmod ug+x script.sh
hacker@chaining~executable-shell-scripts:~$ ls -l script.sh
-rwxr-xr-- 1 hacker hacker 17 Oct 17 18:11 script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{0wikXR1T1djrhWZLNqIpP3AV8mx.dRzNyUDLycjN0czW}
```
## Learnings:
- I learned to create and execute a shell script directly without invoking bash, simplifying by adding execution permissions to the shell script.
## References:
None

