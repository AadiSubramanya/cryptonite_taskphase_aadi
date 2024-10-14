# Suspending Processes
## Code:
```bash
hacker@processes~suspending-processes:~$ /challenge/run
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
Yay, I found another version of me! Here is the flag:
pwn.college{Ae_O2XlseM8VErWY02g8A9O4-4f.dVDN4QDLycjN0czW}
```
## Learnings:
- Suspending processes in the terminal using Ctrl-Z, which sends them to the background.
- For this challenge, I need to start `/challenge/run`, suspend it with Ctrl-Z, and then launch another copy while the first one is suspended.
## References:
None

