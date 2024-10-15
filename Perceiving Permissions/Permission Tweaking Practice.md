Permission Tweaking Practice# 
## Code:
```bash
hacker@permissions~permission-tweaking-practice:~$ /challenge/run
Round 0 (of 8)!
Current permissions of "/challenge/pwn": rw-r--r--
Needed permissions of "/challenge/pwn": rw-r--r-x

hacker@permissions~permission-tweaking-practice:~$ chmod o+x /challenge/pwn
You set the correct permissions!
Round 1 (of 8)!
Current permissions of "/challenge/pwn": rw-r--r-x
Needed permissions of "/challenge/pwn": rw-r--r--

hacker@permissions~permission-tweaking-practice:~$ chmod o-x /challenge/pwn
You set the correct permissions!
Round 2 (of 8)!
Current permissions of "/challenge/pwn": rw-r--r--
Needed permissions of "/challenge/pwn": r--r--r--

hacker@permissions~permission-tweaking-practice:~$ chmod u-w /challenge/pwn
You set the correct permissions!
Round 3 (of 8)!
Current permissions of "/challenge/pwn": r--r--r--
Needed permissions of "/challenge/pwn": r--r-----

hacker@permissions~permission-tweaking-practice:~$ chmod o-r /challenge/pwn
You set the correct permissions!
Round 4 (of 8)!
Current permissions of "/challenge/pwn": r--r-----
Needed permissions of "/challenge/pwn": ---------

hacker@permissions~permission-tweaking-practice:~$ chmod ugo-r /challenge/pwn
You set the correct permissions!
Round 5 (of 8)
Current permissions of "/challenge/pwn": ---------
Needed permissions of "/challenge/pwn": ---rw----

hacker@permissions~permission-tweaking-practice:~$ chmod g+rw /challenge/pwn
You set the correct permissions!
Round 6 (of 8)!
Current permissions of "/challenge/pwn": ---rw----
Needed permissions of "/challenge/pwn": ---------

hacker@permissions~permission-tweaking-practice:~$ chmod g-rw /challenge/pwn
You set the correct permissions!
Round 7 (of 8)!
Current permissions of "/challenge/pwn": ---------
Needed permissions of "/challenge/pwn": ---rwx---

hacker@permissions~permission-tweaking-practice:~$ chmod g+rwx /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! 

hacker@permissions~permission-tweaking-practice:~$ ls -l /flag
---------- 1 hacker hacker 58 Oct 15 05:21 /flag

hacker@permissions~permission-tweaking-practice:~$ chmod ug+r /flag
hacker@permissions~permission-tweaking-practice:~$ cat /flag
pwn.college{EtkCjZtMxvPwp0ASdRYSfU-T4tl.dBTM2QDLycjN0czW}

```
## Learnings:
- I practiced using `chmod` to manipulate read, write, and execute permissions across multiple rounds.
- Each step helped me in understanding what is r,w,x and what is u,g,o.
- Ultimately, I made the `/flag` file readable by correctly modifying its permissions.
## References:
None
