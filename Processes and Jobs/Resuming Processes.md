# Resuming Processes
## Code:
```bash
hacker@processes~resuming-processes:~$ /challenge/run
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{s-DoS6echNSTPiszVPewL2wPK-j.dZDN4QDLycjN0czW}
```
## Learnings:
- Resuming suspended processes using the `fg` command, which brings them back to the foreground.
- For this challenge, I need to suspend `/challenge/run` and then use `fg` to resume it.
## References:
None

