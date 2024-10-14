# Listing Processes
## Code:
```bash
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 15:17 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /ru
root           7       1  0 15:17 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 15:17 ?        00:00:00 /challenge/18661-run-24367
root          72      68  0 15:17 ?        00:00:00 sleep 6h
hacker        73       0  0 15:18 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90      73  0 15:18 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/18661-run-24367
Yahaha, you found me! Here is your flag:
pwn.college{AU_HEdElIVIr3XjuKIjCYb3hbMc.dhzM4QDLycjN0czW}
```
## Learnings:
- I learned to list running processes with the `ps` command.
-  Unlikes and likes between `ps -ef` for details or `ps aux`.
-  For this challenge, I need to find a renamed `/challenge/run` in the process list and relaunch it to get the flag.
## References:
None

