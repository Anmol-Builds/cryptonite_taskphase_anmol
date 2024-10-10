#MODULE 2: Pondering Paths
This module dives a bit deeper into **_finding_ and _locating_** files. It provides a deeper insight on **Absolute and relative Paths and how to access them and Invoke them occassionally**
****
**The Root:**
In this task we were asked to locate and invoke an anbsolute path for the file "**_pwn_**" and this was easily done by me using the command "**_/pwn_**" and I got the flag
****
**Program and Absolute Paths:**
In this task we were told told that all the challenges are in the **challenge directory** and this is located in the "**_root directory: /_**". So we had to go into the root directory fisrt by typing "/" in the terminal and then we had to type "_/challenge_" to go tinto that directory and then I could easily run the command "**_/challenge/run_**" to get the flag
****
**Position thy Self:**
We were told that "_The Linux filesystem"_ has tons of directories with tons of files. You can navigate around directories by using the "**_cd_** (**c**hange **d**irectory) command" and passing a path to it as an argument.
"**_cd_**" is a navigation command which allows us to navigate to aprticualr file in a particular directory in which we have work. I invoked the cd command here to navigate to "**_/challenge_**" by first going into "**_/home_**" and then  **cd**ing into "**_/challenge/run_**" to then get the flag.
****
**Position Elsewhere:**
This is the same challenge as above but we have to "**cd**" into a  different directory.
****
**Position yetelsewhere:**
This is a practical apllication (same as the) previous task
****
**implicit relative paths, from/**
In this task we were tought about relative paths, 
**. A relative path is any path that does not start at root (i.e., it does not start with /).
. A relative path is interpreted relative to your current working directory (cwd).
. Your cwd is the directory that your prompt is currently located at.**
"**_This means how you specify a particular file, depends on where the terminal prompt is located._**"
Here I had to get into the main directory and then I had to do "_/challenge/run_" but
I faced a problem in accessing the directory using relative paths as I was not very familiar with how to access a directory using relative path.Then I understood that relative path removes the "_/_" out of the way and there fore the command begins with "c" and I understood the basc concept of relative path and I got the flag by entering the command ***challenge/run***.

**explicit relative paths, from/: **
In most operating systems, including Linux, every directory has two implicit entries that you can reference in paths: . and ... The first, ., refers right to the same directory, so the following absolute paths are all identical to each other:

**1)/challenge
2)/challenge/.
3)/challenge/./././././././././
4)/./././challenge/././**

In this task we tought how to access challenges inside directories using "." (implicit way of accessing a challenge) I had to cd into "**/**" folder and then run ***"./challenge/run"*** to get the flag.
****
**Implicit relative path**
In this challenge we had to run the challenge/run implicitly. In order to get the flag we have to cd into "**/**" and then we had to execute the command: ***./run*** .
****
**Home sweet home**
in this task we learn the meaning of ~ which is the shorthand of /home
using this we cd into /home/hacker using ***cd ~*** command and then after this we run ls command to find out there is only "a" so therefore you run the command "**/challenge/run ~/a**" to get the flag


