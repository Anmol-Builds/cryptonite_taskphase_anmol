#MODULE 3: comprehending commands
This module exposes us to basic but useful commands of linux like **cat**, **grep**, **touch**, etc. this program was easy at first but there were some questions which required a lot of thinking(atleast for me)
****
**cat: not the pet, but the command!** In this task cat function was briefly explained and then we were asked to copy the flag to the flag file in your home directory (where your shell starts) and then read it with cat
This was very basic and i did it using **'cat ~/flag'**
****
**catting absolute paths** this was similar to the last question but this time system did not copy it to the home directory, but I made it readable
to read the flag, we used the **'cat /flag'** command
****
**more catting practice** this was also similar to last question but this time it was not allowed to change directories with cd so i did it using absolute path
there was already a path provided so i just read it using catenate
**cat /lib/locale/flag**
****
**grepping for needle in haystack** this question explained about the grep function and then asked a pretty simple question on it. the hint provided was very helpful in this question and the piping module
**grep "pwn.college" /challenge/data.txt**
****
**listing files** this question got a bit confusing as knew the initial and final steps but one step was missing
i used **ls /challenge** which got me a file named **9913-renamed-run-30493**, i did not know how to open it so i opened it from the file manager which gave the final command i.e. **cat ~/flag** but it did not run as final steps were missing 
****
**touching files** this program was very straight forward i dont think there is a need to explain it and shantanu sir has also approved it.
****
**removing file** this program was very straight forward i dont think there is a need to explain it and shantanu sir has also approved it.
****
**an epic file system quest** this was a very easy but tiring program, the only tricky part was the one where the flag could have self destructed(my file got destructed 4 times)
the input was
cd /
ls -a 
then it would provide files in CAPITAL LETTERS that is the clue cat it 
this would repeat for a long time some times without cding into the directory sometimes by using -a or sometimes without using cat
eventually it gave the flag
****
**making directories ** this program was very straight forward i dont think there is a need to explain it and shantanu sir has also approved it.
****
**finding files** this was very tricky for me and i was not able to obtain the flag i will share what i thought during the process
**find / -name flag** to list the files with flag 
after this i individually opened all the files but none of them had the flag 
i was not able to find the solution for this even after reffering youtube, geeksforgeeks,chatgpt
****
**linking files** i was not able to solve this as it needed prior knowledge of finding files program
****
end

   
