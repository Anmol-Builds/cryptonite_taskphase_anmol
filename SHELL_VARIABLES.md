#MODULE 7: shell variables  
****
**printing variables** this was very straight forwardand easy 
**code:**
hacker@variables-printing-variables:-$ echo $FLAG
pwn.college{M3hfAFZJkwiUfFnQfeffFHcR4ff.ddTN1QDLxAzN0czW}

****
**setting variables** this was very straight forwardand easy 
**code:** 
hacker@variables-setting-variables:~$ PWN=COLLEGE
You've set the PWN variable properly! As promised, here is the flag: pwn.college{c8PG2orfgoNzW0Xdz5h8MF60r8G.dlTN1QDLxAzN0czW}
****
**MULTIWORD VARIABLES** this was very straight forwardand easy 
**code**
hacker@variables~multi-word-variables:~$ PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag: pwn.college{MXF4i_xKmecVG3ThpfYvcggq3LD.dBjN1QDLxAzN0czW}
****
**exporting variables** this was very straight forward and easy 
**code** 
hacker@variables-exporting-variables:~$ COLLEGE=PWN
You've set the COLLEGE variable to the proper value!
hacker@variables-exporting-variables:~$ export PWN COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:-$ /challenge/run
CORRECT!
You have exported PWN COLLEGE and set, but not exported, COLLEGE=PWN. Great job! Here is your flag:
pwn.college{8hmsNObfH2IHEp9Hi29Ri8TJuzk.dJjN1QDLxAzN0czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
****
**printing exported variables** this was very straight forward and easy but searching for the FLAG was a task
**code:**
**env**
now it printed lots of variables through which i found the flag = **"4g9Qx8gq11D0APGsvyz2YdCoENJ.dhTN1QDLxAzN0czW"**

****
**storing command output** Just followed what was told 
**code:**
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run )
Congratulations! You have read the flag into the PWN variable. Now print it out and submit it!
hacker@variables~storing-command-output: and-output:~$ echo $PWN
pwn.college{Q1jLzJSNFm0eDRFup0jBYW4ivoB.dVzNOUDLxAzN0czW}
****
**reading input** answer was one line as i just followed what was told 
**code:**
hacker@variables-reading-input:~$ read -p "Input" PWN
InputCOLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{ICbd223jFQVL8GyV_Iw7910x6L1.dhzN1QDLxAzN0czW}
****
**reading files** it took some tries for me to get to the flag 
**code**
hacker@variables-reading-files:~$ cd /challenge/
hacker@variables-reading-files:/challenges read PWN < read_me 
You've set the PWN variable properly! As promised, here is the flag: pwn.college{UIsEQIw43-bPZa31rD-TW-nWOpt.dBjM4QDLxAzN0czW} 
****

 End












   
