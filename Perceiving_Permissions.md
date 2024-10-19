#MODULE 9:Perceiving Permissions
  
****
**changing file ownership** this was very straight forward and easy but i got to learn a lot  
**code:**
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions-changing-file-ownership:-$ cat /flag 
pwn.college{Q97LhYPfkUpYU6HnflAxS7gY63Q.dFTM2QDLxAzN0czW}

****
**groups and files** this was very straight forward and easy 
**code:** 
hacker@permissions-groups-and-files:-$ chgrp hacker /flag
hacker@permissions-groups-and-files:-$ cat /flag
pwn.college{AXrNfX2LJ00WN62a6HTRfAfDl8z.dFzNyUDLxAzN0czW}
hacker@permissions-groups-and-files:~$
****
**fun with group names** this was very straight forward and easy 
**code**
hacker@permissions-fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp19254) groups=1000(grp19254)
hacker@permissions-fun-with-groups-names:-$ chgrp grp19254 /flag
hacker@permissions-fun-with-groups-names:~$ cat /flag 
pwn.college{w-kfs4DzIwJmqNl1P2LM-2Qc5QH.dJzNyUDLxAzN0czW}
****
**changing permissions** i was having problems in this question, i think there was issue with the terminal as after repeating the same commands again and again i got the flag 
**code** 
hacker@permissions~changing-permissions:~$ chmod +rwx /flag
hacker@permissions~changing-permissions:~$ id
uid=1000(hacker) gid=1000 (hacker) groups 1000 (hacker)
hacker@permissions-changing-permissions:~$ ls -l /flag
-rwxr-xr-x 1 root root 58 Oct 19 08:57 /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{QtDP5Yj4dYfgqed44fuK8bV1f1r.dNzNyUDLxAzN0czW}

i was thinking of other ways that is why i used id and ls -l /flag
****
**executable files** 
**code:**
hacker@permissions-executable-files:~$ chmod +x /challenge/run
hacker@permissions-executable-files:~$ /challenge/run
bash: /challenge/run: Permission denied
hacker@permissions-executable-files:~$ ls -l /challenge/run
-r--r--r-x 1 hacker hacker 32 Jul 4 06:37 /challenge/run 
hacker@permissions-executable-files:~$ chmod ugo+x /challenge/run
hacker@permissions-executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{glD4zw9cFh0639VgtTeK4gUdLyn.dJTM2QDLxAzN0czW}

****
**permission tweaking practice** i have not written the output code as it was very big 
**code:**
/challenge/run 
hacker@permissions-permission-tweaking-practice:~$ chmod o-r /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod ug-r /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod go+rw /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod ug-w /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod uo+x /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod o-rw /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod uo+rw /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod ug-rwx /challenge/pwn
hacker@permissions-permission-tweaking-practice:~$ chmod ugo+r /flag
hacker@permissions-permission-tweaking-practice:~$ chmod cat /flag
this gave the flag

****
**permission setting practice** it was easy but very tedious 
**code:**
to make less effort i just overwrote all the perms by using **=**
some questions also required the use of **-**
this gave the flag 4LNAX2eVAnmDABJyyh0kNxVbULV.dNTM5QDLxAzN0czW
****
**The SUID bit** 
**code:**
hacker@permissions-the-suid-bit:~$ chmod ugo+s /challenge/getroot
hacker@permissions-the-suid-bit:~$ cat /challenge/getroot
#!/opt/pwn.college/bash
fold -s <<< "SUCCESS! You have set the suid bit on this program, and it is running as root! Here is your shell..."
exec /bin/bash
hacker@permissions-the-suid-bit:~$ /bin/bash hacker@permissions-the-suid-bit:-$/challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell
root@permissions-the-suid-bit:~# cat /flag
pwn.college{U0kxijA69xtMgDE4zyLaJyn6_tj.dNTM2QDLxAzN0czW}
****

 End












   
