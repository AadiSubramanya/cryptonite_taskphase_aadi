# Cracking Passwords
## Code:
```bash
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04819g/s 280.6p/s 280.6c/s 280.6C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{Q8RizV8dziBNfI_92s2gHjuXYz9.ddTN0UDLycjN0czW}
```
## Learnings:
- User passwords are now stored in `/etc/shadow` instead of `/etc/passwd` for security reasons.
- The `su` command checks the hashed password against the stored hash in `/etc/shadow` when attempting to switch users.
- I simulated cracking a leaked password hash using John the Ripper, which revealed Zardus' password, allowing me to switch users and retrieve the flag.
## References:
None

