# Groups and Files
## Code:
```bash
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{AcuRvCUS_IujtongFFmQO_8lz1j.dFzNyUDLycjN0czW}
```
## Learnings:
- Changing group ownership in Linux. I changed the group of the `/flag` file to `hacker` using `chgrp hacker /flag`, which allowed me to read the flag.
- This highlighted the importance of group permissions in accessing files.
## References:
None

