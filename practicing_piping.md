#MODULE 6: practicing piping 
this was the toughest module in all of the modules, initial questions were easy but the latter were very hard to crack 
****
**redirecting output** this was very straight forwardand easy 
code **echo PWN > COLLEGE**
****
**redirecting more output** this was very straight forwardand easy 
code **/challenge/run > myflag**
**cat myflag**
****
**appending output** this was very straight forwardand easy 
code 
/challenge/run >> /home/hacker/the-flag
cat /home/hacker/the-flag
****
**redirecting errors** this was very straight forwardand easy 
code 
/challenge/run > myflag 2> instructions
cat myflag
****
**redirecting input** this was very straight forwardand easy 
code 
echo COLLEGE > PWN
/challenge/run < PWN
now recalled using echo to get flag 
****
**grepping stored results**
this is where things started getting tough for me 
after a very long time and consulting many friends i got to know that i had to use pwn.college while grepping as mentioned in module 3 
then i was able to solve it 
/challenge/run > /tmp/data.txt
grep "pwn.college" /tmp/data.txt
****
**grepping live output** very tricky even tough answer was one line 
/challenge/run echo | grep "pwn.college"
****
**duplicating piped data with tee** toughest of them all 
code 
/challenge/pwn | tee --cmd1_output | /challenge/college
cat cmd1_output    this gave the secret value IOC9q4Ls
/challenge/pwn --secret IOC9q4Ls | /challenge/college
this gave the flag 
****
i was not able to solve the rest 3 problms and they were somwhat interrelated and complex , however i will research more and work on them 
****
 end












   
