# Killing Processes
## Code:
```bash
hacker@processes~killing-processes:~$ ps -ef | grep /challenge/dont_run
hacker        73      71  0 15:21 ?        00:00:00 /challenge/dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{IJKLQGiJp0br4GeBKxcBBvZJI5K.dJDN4QDLycjN0czW}
```
## Learnings:
- Terminating processes in Linux using the `kill` command by providing the process ID (PID).
- To find a process, I can use `ps` and `grep`, which took me some time to realize, since I didnt think of redirecting output and then grepping it, instead was manually doing it which takes a lot of time.
- For this challenge, I need to locate the `dont_run` process and kill it to allow `/challenge/run` to execute.
## References:
None

