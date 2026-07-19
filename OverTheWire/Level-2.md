\#Bandit Level 2



**Challenge**

Find the password for next level  is stored in file named - , located in home directory



**Approach** 

First I connected to Level 1 using SSH with the password found in Level 0. Then I listed the files in the home directory and found a file named "-". I used "cat ./-" instead of "cat -" because the dash symbol has a special meaning in Linux and cannot be read directly.



**Commands** 

ssh bandit1@bandit.labs.overthewire.org -p 2220

ls

Cat ./-



**What I Learned** 

* How to read if file named "-" with "cat" using "./-", because "-" means standard input in Linux



**Key Takeaway**

In Linux some filenames have special meanings. Using "./" before a filename forces Linux to treat it as a file — important skill in cybersecurity when dealing with unusual filenames.



