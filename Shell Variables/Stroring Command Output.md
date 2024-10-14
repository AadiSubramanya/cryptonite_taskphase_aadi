# Storing Command Output
## Code:
```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{Q1eHEw1ptvzgv53UFOFMrHinDeo.dVzN0UDLycjN0czW}
```
## Learnings:
- I learned how to store the output of a command in a variable using command substitution, like `PWN=$(command)`.
- Took me some time to realize I have to use the $ sign to store the output from the command.
- For this challenge, get output from `/challenge/run` into the `PWN` variable and then print it out to find the flag.
## References:
None
