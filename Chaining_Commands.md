#MODULE 11:Chaining Commands

****
**chaining with semicolons** this was straight forward 
**code:** 
hacker@chaining-chaining-with-semicolons:~$ /challenge/pwn; /challenge/college
Yes! You chained /challenge/pwn and /challenge/college! Here is your flag: 
pwn.college{YgfQIdDgjXrObXBHrKjwbxza_p8.dVTN4QDLxAzN0czW}
****
**your first shell script** 
i was not able to solve this question through terminal. I think i was making a mistake in the commands 
to solve the question i manually opened x.sh from file manager, entered /challenge/pwn and /challenge/college
then executed bash x.sh in terminal to get the flag
****
**redirecting script output** 
**code** 
hacker@chaining-redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{QWh01NilufSIIx801rOtB8NA4QW.dhTM5QDLxAzN0czW}
****
**executable shell scripts**
**code**
hacker@chaining-executable-shell-scripts:~$ ls -l x.sh
-rw-r--r-- 1 hacker hacker 18 Oct 19 12:26 x.sh
hacker@chaining-executable-shell-scripts:~$ chmod ugo+x x.sh
hacker@chaining-executable-shell-scripts:~$ /x.sh
bash: /x.sh: No such file or directory
hacker@chaining-executable-shell-scripts:~$ ./x.sh
Congratulations on your shell script execution! Your flag: 
pwn.college{M4bYTKTOXJT_OqcB_4kk23P0tpL.dRzNyUDLxAzN0czW}
****

 End












   
