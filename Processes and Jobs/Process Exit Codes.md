# Process Exit Codes
## Code:
```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
168
hacker@processes~process-exit-codes:~$ /challenge/submit-code 168
CORRECT! Here is your flag:
pwn.college{s_gGooIIvwQLwMjNEzTSyFQq782.dljN4UDLycjN0czW}
```
## Learnings:
- Every shell command exits with a code indicating success (0) or failure (non-zero).
- I can check the exit code of the last command using the `$?` variable.
- For this challenge, I need to run `/challenge/get-code`, retrieve its exit code, and then use that code as an argument for `/challenge/submit-code`.
## References:
None

