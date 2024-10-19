# Setting PATH
## Code:
```bash
hacker@path~setting-path:~$ ls /challenge/run
/challenge/run
hacker@path~setting-path:~$ ls /challenge/more_commands/
win
hacker@path~setting-path:~$ PATH=/challenge/more_commands/
hacker@path~setting-path:~$ win
It looks like 'win' was improperly launched. Don't launch it directly; it MUST
be launched by /challenge/run!
hacker@path~setting-path:~$ /challenge/run/win
ssh-entrypoint: /challenge/run/win: Not a directory
hacker@path~setting-path:~$ PATH=/challenge/more_commands/
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{AUDcX8hxFncoSWLV5zUkVuCWr5G.dVzNyUDL0kTN0czW}
```
## Learnings:
- First i didnt get this but after trying again i got it that we where trying to use the win by using /challenge/run.
## References:
None

