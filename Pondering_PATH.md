#MODULE 12: Pondering PATH

****
**the PATH variable** this question required some thinking and references to solve  
**code:** 
hhacker@path-the-path-variable:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/
usr/bin:/sbin:/bin
hacker@path-the-path-variable:~$ mkdir tempdirectory
hacker@path-the-path-variable:~$ export PATH=$(/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin)/tempdirectory
bash: /run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin: No such file or directory
hacker@path-the-path-variable:~$ export PATH=$(pwd)/tempdirectory
hacker@path-the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: command not found
The flag is still there! I might as well give it to you!
pwn.college{oMNcGD4cNbxBRQ4-tS-LhY3jyUk.dZzNwUDLxAzN0czW}
****
**setting PATH** 
**code**
hacker@path-setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'.
Congratulations! You properly set the flag and 'win' has launched! 
pwn.college{MnRPvqytzrNgqyiwKOSB1GA7y6P.dVzNyUDLxAzN0czW}
****
**adding comaands** 
not able to solve this question 
****
**hijacking commands**
not able to solve this question 
****

 End












   
