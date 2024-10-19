#MODULE 10: Untangling Users
  
****
**becoming root with su** this was very straight forward and easy 
**code:**
hacker@users-becoming-root-with-su:~$ su
Password:
root@users-becoming-root-with-su:/home/hacker# /flag
bash: /flag: Permission denied
root@users-becoming-root-with-su:/home/hacker# cat /flag 
pwn.college{8HicUmzMJqnbRppp1KQTDR2Kigu.dVTNOUDLxAzN0czW}
root@users-becoming-root-with-su:/home/hacker#

****
**other user with su** this was very straight forward and easy 
**code:** 
hacker@users-other-users-with-su:~$ su zardus
Password:
zardus@users-other-users-with-su:/home/hacker$ /challenge/run 
Congratulations, you have become Zardus! Here is your flag: 
pwn.college{0K5XfB7TZ0XFEJtvXq2tWQI9tG9.dZTN0UDLxAzN0czW}
****
**cracking passwords** 
**code:**
hacker@users-cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status 
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04967g/s 289.2p/s 289.2c/s 289.2C/s Johnson..buzz 
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users-cracking-passwords:~$ --show
bash:show: command not found
hacker@users-cracking-passwords:~$ su zardus
Password:
zardus@users-cracking-passwords:/home/hacker$ /challenge/run 
Congratulations, you have become Zardus! Here is your flag: 
pwn.college{cUlLYF9o1x_MCb1ryeBNc3D9hR3.ddTNOUDLxAzN0czW}
****
**using sudo** 
**code** 
hacker@users-using-sudo:~$ sudo cat /flag
pwn.college{wjzaOFnStcadcZGCcjm6wwWHljO.dhTN0UDLxAzN0czW}
****


 End












   
