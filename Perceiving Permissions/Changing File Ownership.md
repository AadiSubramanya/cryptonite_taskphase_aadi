# Changing File Ownership
## Code:
```bash
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{scurt1b3wgTBpM2pgKOwil2Z9Q8.dFTM2QDLycjN0czW}
```
## Learnings:
- File ownership can be changed in Linux using the `chown` command.
- By changing the ownership of the `/flag` file from `root` to my user account, I was able to access its contents successfully.
- Highlighted the importance of understanding file permissions and ownership.
## References:
None

