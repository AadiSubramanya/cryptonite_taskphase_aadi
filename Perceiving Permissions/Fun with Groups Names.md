# Fun with Groups Names
## Code:
```bash
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp22807) groups=1000(grp22807)
hacker@permissions~fun-with-groups-names:~$ chgrp grp22807 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{ACR8LjoymlFjlEiBZ0-dIwWOoOm.dJzNyUDLycjN0czW}
```
## Learnings:
- This exercise reinforced the importance of checking user group information to access files correctly.
- Using the `id` command, I discovered my group name was randomized as `grp22807`. I then changed the group ownership of the `/flag` file to match this group using `chgrp grp22807 /flag`. This allowed me to successfully read the flag.
## References:
None

