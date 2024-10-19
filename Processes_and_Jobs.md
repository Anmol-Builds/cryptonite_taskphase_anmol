#MODULE 8: Processes and Jobs
  
****
**Listing processes** this was very straight forward and easy but i got to learn a lot  
**code:**
ps aux
hacker@processes-listing-processes:~$ /challenge/15397-run-8837
Yahaha, you found me! Here is your flag:
pwn.college{kBgV8UvWDgaD3t5X8GYAx9P21rL.dhzM4QDLxAzN0czW}
Now I will sleep for a while (so that you could find me with 'ps')

****
**killing processes** this was very straight forwardand easy 
**code:** 
ps aux
hacker@processes-killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{w94o1jhGp2z-Y_9rqfbrtf4HuAX.dJDN4QDLxAzN0czW}
****
**interupting processes** this was very straight forwardand easy 
**code**
hacker@processes-interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember, you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag: pwn.college{wG8GmLiqKlDjP10DgjWABP5kQyk.dNDN4QDLxAzN0czW}
****
**suspending processes** this was very straight forward and easy 
**code** 
hacker@processes~suspending-processes:~$ /run
bash
: /run: Is a directory
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in this terminal... Let's check!

I don't see a second me!
To pass this level, you need to suspend me and launch me again! You can background me with Ctrl-Z or, if you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+ Stopped           /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in this terminal... Let's check!

Yay, I found another version of me! Here is the flag: pwn.college{gACqf1kZEE7c9WbVt60lJD5MUFB.dVDN4QDLxAzN0czW}
****
**resuming processes** 
**code:**
hacker@processes-resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with the 'fg' command! Or just press Enter to quit me!
^Z
[1]+ Stopped
/challenge/run
hacker@processes-resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{IFJOQgwanXOJ9f4-uCkkDREw76T.dZDN4QDLxAzN0czW}
Don't forget to press Enter to quit me!

Goodbye!!

****
**backgrounding processes** i have not written the output code as it was very big 
**code:**
/challenge/run 
ctrl+z
bg
/challenge/run
****
**foregrounding processes** I just followed what was told 
**code:**
hacker@processes-foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the background, and *then* foreground it without re-suspending it! You can background me with Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+ Stopped
/challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+/challenge/run &
hacker@processes~foregrounding-processes:~$ Yay, I'm now running the background! Because of that, this text will probably overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.
hacker@processes~foregrounding-processes:~$ fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!
pwn.college{gu5cAVOcK0rQ899z-o9yTqxBEqU.dhDN4QDLxAzN0czW}
****
**starting background processes ** 
**code**
hacker@processes-starting-backgrounded-processes:~$ /challenge/run &
[1] 337
hacker@processes-starting-backgrounded-processes:~$
Yay, you started me in the background! Because of that, this text will probably overlap weirdly with the shell prompt, but you're used to that by now...
Anyways! Here is your flag!
pwn.college{cMZhuztNUf4Z6XymJkyE_YyRGeC.dlDN4QDLxAzN0czW}
****
**process exit codes**
**code**
hacker@processes-process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes-process-exit-codes:~$ echo $?
38
hacker@processes-process-exit-codes:~$ /challenge/submit-code 38
CORRECT! Here is your flag: pwn.college{00J9EfFMDmHConzs3Fsc8NrRi8Y.dljN4UDLxAzN0czW}
****
 End












   
