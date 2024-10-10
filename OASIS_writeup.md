# Heads up, Tails down
Got an image that was corrupted, knew that we had to fix it. We tried understanding how png image data is formatted, and found out that its writted on hexadecimal data type. 
Tried all techniques to convert the enrpted data (image data) into normal hexadecimal and still didnt get the fixed image.
We then realized we had to "fix" the image, so we looked up the exact format for hexacode of a image and fixed the format of the given image and we had a proper image that led us to the flag


# I have been falling for 30 minutes!
Got a website and knew we had to somehow break the firewall to reach the flag.
Tried all cheap tricks like inspect element but nothing worked.
Approached the question in a different way by examining the url, which had a parameter user_id = x (ranged from 1 to 5)
Simply tried manually putting in 6 in the user id and low and behold it led to the flag


# Stairway to Heaven
Recieved a game.file from the challenge, took us a long time of trying all de-encryting files just to realize it was a linux executable file
Ran the file through a terminal and got a pixelated image
Since the image itself had no hidden code, we tried to copy and paste it.
It pastedin the form of text in which the flag was hidden


# Git Gud
Very honestly, brute forces though all files and found the flag hidden in one of the files


# Quence your thirst
One of the most beautifull challenges in my opinion
Following the hint given in the discord server, we ran the given text through a text frequency analyzier
Brute forced out way through the likely letters and finally found the link with 4 missing letters (j,q,x,z)
Found all the possible combinations of the letters in the missing spot and finally found the right link with led to the flag
