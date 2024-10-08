# Reading Manuals
## Code:
```bash

hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                                   Challenge Commands                                                   CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --tpmbso NUM
              print the flag if NUM is 210

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                         May 2024                                                        CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge --tpmbso 210
Correct usage! Your flag: pwn.college{QXJt2pmbso10cBcM44GkroSjUIP.dRTM4QDLycjN0czW}
```
## Learnings:
Understanding commands and arguments

## References:
None

