# Backgrounding Processes
## Code:
```bash
hacker@processes~backgrounding-processes:~$ /challenge/run
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg
hacker@processes~backgrounding-processes:~$ /challenge/run
Yay, I found another version of me running in the background! Here is the flag:
pwn.college{cfLL6P4TvmjGVZUj_WCEbcj8LIM.ddDN4QDLycjN0czW}
```
## Learnings:
- Resuming suspended processes in the background using the `bg` command, which lets the process continue running while I regain access to the shell.
- For this challenge, I need to launch `/challenge/run`, suspend it, background it with `bg`, and then launch another copy while the first one runs in the background
## References:
None

