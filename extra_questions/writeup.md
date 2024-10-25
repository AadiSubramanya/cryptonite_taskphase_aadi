Level 0:
Code:
ssh bandit0@bandit.labs.overthewire.org -p 2220
pswd:bandit0

writeup
Logging into the OverTheWire game using SSH with specified credentials to progress to the next level.





Level 0-1:
Code:
cat readme
pswd:ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

writeup
used ssh to log into level 1 and then cat the readme file to get the password.
noted that you have to logout after finding password and log into next level using ssh and password.





Level 1-2:
Code:
cat readme
pswd:263JGJPfgU6LtdEvgfWU1XP5yac29mFx

writeup
used ssh to log into level 1 and then cat the readme file to get the password.
noted that you have to logout after finding password and log into next level using ssh and password.





Level 2-3:
Code:
cat "spaces in this filename"
pswd:MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

writeup
used quotes to read the file name as a single token






Level 3-4:
Code:
bandit3@bandit:~$ cd inhere
bandit3@bandit:~/inhere$ ls -a
.  ..  ...Hiding-From-You
bandit3@bandit:~/inhere$ cat "...Hiding-From-You"
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

writeup
cd to given directory and then used quotes to read the file name as a single token







Level 4-5:
Code:
bandit4@bandit:~$ cd inhere
bandit4@bandit:~/inhere$ ls -a
.  ..  -file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ 	
 p  & y , (jo .at :uf ^   @i R , Λ :Y   ? % A    B  ͩ 3          )Ʈ #Y  -6c  IR- $    :     / 
                                                                                                    qGi  , 2 Yb 
dۙ rOx    h0~ey
  c ~ h n  G1}   ߓ  ߤ  W>  #lk d ܮ  yE  6 0] \ $ 1 %       o@  b/  4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
 nS 
 <  ] 
W  e ˥m     O  D  2g  ?     `>5HYA u   8 g `0 $`  b

writeup
cd to given directory and then cat all similar format files at one command






Level 5-6:
Code:


writeup
cd to given directory and then cat all similar format files at one command
