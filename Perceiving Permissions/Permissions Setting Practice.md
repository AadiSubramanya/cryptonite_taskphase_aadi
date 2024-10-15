# Permissions Setting Practice
## Code:
```bash
hacker@permissions~permissions-setting-practice:~$ /challenge/run
Round 0 (of 8)!
Current permissions of "/challenge/pwn": rw-r--r--
Needed permissions of "/challenge/pwn": rw-r-xr--

hacker@permissions~permissions-setting-practice:~$ chmod g+x /challenge/pwn
You set the correct permissions!
Round 1 (of 8)!
Current permissions of "/challenge/pwn": rw-r-xr--
Needed permissions of "/challenge/pwn": -wx----wx

hacker@permissions~permissions-setting-practice:~$ chmod uo=wx,g=- /challenge/pwn
You set the correct permissions!
Round 2 (of 8)!
Current permissions of "/challenge/pwn": -wx----wx
Needed permissions of "/challenge/pwn": r--r-xr-x

hacker@permissions~permissions-setting-practice:~$ chmod u=r,go=rx /challenge/pwn
You set the correct permissions!
Round 3 (of 8)!
Current permissions of "/challenge/pwn": r--r-xr-x
Needed permissions of "/challenge/pwn": r--r-xrw-

hacker@permissions~permissions-setting-practice:~$ chmod o=rw /challenge/pwn
You set the correct permissions!
Round 4 (of 8)!
Current permissions of "/challenge/pwn": r--r-xrw-
Needed permissions of "/challenge/pwn": ----wxrw-

hacker@permissions~permissions-setting-practice:~$ chmod u=-,g=wx /challenge/pwn
You set the correct permissions!
Round 5 (of 8)!
Current permissions of "/challenge/pwn": ----wxrw-
Needed permissions of "/challenge/pwn": rwxr-xrw-

hacker@permissions~permissions-setting-practice:~$ chmod u=rwx,g=rx /challenge/pwn
You set the correct permissions!
Round 6 (of 8)!
Current permissions of "/challenge/pwn": rwxr-xrw-
Needed permissions of "/challenge/pwn": rw---x--x

hacker@permissions~permissions-setting-practice:~$ chmod u=rw,go=x /challenge/pwn
You set the correct permissions!
Round 7 (of 8)!
Current permissions of "/challenge/pwn": rw---x--x
Needed permissions of "/challenge/pwn": -w-r-x-wx

hacker@permissions~permissions-setting-practice:~$ chmod u=w,g+r,o+w /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds!

hacker@permissions~permissions-setting-practice:~$ ls -l /flag
---------- 1 hacker hacker 58 Oct 15 05:35 /flag

hacker@permissions~permissions-setting-practice:~$ chmod ugo=r /flag
hacker@permissions~permissions-setting-practice:~$ cat /flag
pwn.college{wrs-diBYD0ODH2ceaPgjzEbFK3Z.dNTM5QDLycjN0czW}

```
## Learnings:
- Learnt how to set file permissions using chmod with the = operator, which overwrites existing permissions, as opposed to simply adding or removing them with + and -.
- This reinforced my understanding from the previous challenge while introducing the concept of chaining permissions for different user categories using ','.
-  Also taught me you can zero out permissions with o=- for example.
## References:
None

