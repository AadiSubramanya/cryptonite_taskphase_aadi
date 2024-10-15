# Becoming Root with SU
## Code:
```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{gZrPb-nLnCGVv63pDZ7MdgcB-m2.dVTN0UDLycjN0czW}
```
## Learnings:
- The `su` command, allows users to switch to the root account.
- The `su` binary has the SUID bit set, enabling it to run with root privileges.
- To successfully elevate to root, I needed the root password, which is "hack-the-planet" in this challenge. After entering the password, I accessed the flag as the root user.
## References:
None

