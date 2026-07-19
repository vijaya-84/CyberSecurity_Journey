\#Bandit Level 3







Challenge



The password for the next level is stored in a file called --spaces in this filename-- located in the home directory







Approach 



First I connected to Level 2 using SSH command with the password which I found in Level 1. Then I listed the files in the home directory and found a file named "--spaces in this filename--". I used "cat -- "--spaces in this filename--" " instead of "cat "--spaces in this filename--" " because the doble dash symbol has a special meaning in Linux and cannot be read directly.







Commands - 



ssh bandit2@bandit.labs.overthewire.org -p 2220



ls



cat -- "--spaces in this filename--" 



cat ./--spaces\\\\ in\\\\ this\\\\ filename--







What I Learned 



\* How to read file named "--spaces in this filename--" with "cat" 

\* What is the "special character" issue 







Key Takeaway 



In Linux some filenames have special meanings. Using "./" or "--" before a filename forces Linux to treat it as a file ,important skill in cybersecurity when dealing with unusual filenames.













