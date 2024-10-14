# Foregrounding Processes
## Code:
```bash
hacker@processes~foregrounding-processes:~$ /challenge/run
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
hacker@processes~foregrounding-processes:~$ fg
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{c3Rgyr_ZKeOdoc8vuuCaaAUEWw9.dhDN4QDLycjN0czW}
```
## Learnings:
- Bringing a backgrounded process back to the foreground using the `fg` command, just like I do with suspended processes.
- Really cleared the concept and difference in fg and bg processes.
- This allows me to interact with the process again. In this challenge, I'll practice foregrounding a backgrounded process.
## References:
None

