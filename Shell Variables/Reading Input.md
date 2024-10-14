# Reading Input
## Code:
```bash
hacker@variables~reading-input:~$ read -p "Input: " PWN
Input: COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{U6ZWxL1QdOyatkVHkS-G728VC99.dhzN1QDLycjN0czW}
```
## Learnings:
- Using the `read` command to take user input in the shell.
- I can specify a prompt with `-p`, like `read -p "INPUT: " MY_VARIABLE`.
- For this challenge, I need to use `read` to set the variable `PWN` to `COLLEGE`.
## References:
None
