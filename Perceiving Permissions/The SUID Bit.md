# The SUID Bit
## Code:
```bash
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{YHNIsmjiOIW8_YZICgPaIbK12LY.dNTM2QDLycjN0czW}
```
## Learnings:
- The Set User ID (SUID) permission, lets non-root users run programs with the owner's privileges.
- By setting the SUID bit on `/challenge/getroot` with `chmod u+s`, I enabled it to execute as root, allowing me to read the flag.
- This concept is essential for granting access without constant root intervention, but it can introduce security risks.
## References:
None

