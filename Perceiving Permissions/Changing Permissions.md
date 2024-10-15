# Changing Permissions
## Code:
```bash
hacker@permissions~changing-permissions:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~changing-permissions:~$ chmod go+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{ABb14BuB8wRXg1AjrMY-WNrW1XI.dNzNyUDLycjN0czW}
```
## Learnings:
- Modified file permissions with `chmod`.
- Initially, I got a "Permission denied" error when trying to read `/flag,` which made me realize I needed to change its permissions.
- After using `chmod go+r /flag` to add read access, I could successfully read the flag.
- This reinforced my understanding of the importance of file permissions.
## References:
None

