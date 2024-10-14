# Exporting Variables
## Code:
```bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{EO51SgYjhpE84Kb27txh8859LPt.dJjN1QDLycjN0czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```
## Learnings:
- I learned that variables set in a shell are local to that session and won't be inherited by child processes.
- To share a variable with child processes, I need to export it using `export VAR`.
- For this challenge, I need to export the `PWN` variable with the value `COLLEGE` and set the `COLLEGE` variable to `PWN` without exporting it.
## References:
None
