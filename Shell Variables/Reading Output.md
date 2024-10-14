# Reading Output
## Code:
```bash
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{U6ELYGb5ivLgWJHicxnZRMbj5tw.dBjM4QDLycjN0czW}
```
## Learnings:
- Learnt that instead of using `cat` to read a file into a variable, I can use input redirection with the `read` command.
- By doing `read VAR < filename`, I can directly read the contents of a file into a variable.
- For this challenge, I need to read `/challenge/read_me` into the `PWN` variable to get the flag.
## References:
None
