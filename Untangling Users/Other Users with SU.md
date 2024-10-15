# Other Users with SU
## Code:
```bash
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{oIoCsdH5PXC7M1lu9j7Biznm8NC.dZTN0UDLycjN0czW}
```
## Learnings:
- The `su` command can be used to switch to any user by specifying their username.
- After authenticating with the zardus user’s password, "dont-hack-me," I successfully switched users. Once logged in as zardus, I ran the `/challenge/run` program to retrieve the flag.
## References:
None

