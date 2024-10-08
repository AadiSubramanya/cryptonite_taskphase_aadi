# Help for builtins
## Code:
```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "EtLO002J".
hacker@man~help-for-builtins:~$ challenge --secret EtLO002J
Correct! Here is your flag!
pwn.college{EtLO002Jd_Gb9P0HDpjMUMYviKn.dRTM5QDLycjN0czW}
```
## Learnings:
Understanding commands and arguments

## References:
None

