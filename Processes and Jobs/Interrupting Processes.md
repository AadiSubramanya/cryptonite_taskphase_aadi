# Interrupting Processes
## Code:
```bash
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{caTGYWk6B2Ldtdli-ryTqE-Gom3.dNDN4QDLycjN0czW}
```
## Learnings:
- Using Ctrl+C to interrupt and terminate processes running in the terminal. 
- This sends an "interrupt" signal, allowing the application to exit cleanly.
- For this challenge, I need to use Ctrl+C to interrupt `/challenge/run` to get the flag.
## References:
None

