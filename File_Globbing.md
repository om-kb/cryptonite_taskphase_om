# File Globbing

## Challenge 1:Matching with *
leared how to use the * method of file globbing,similar to the . we place before a string in a regular expression that I used before.

This challenge required me to cd into /challenge while using less than 4 charachters so I ran cd /ch* successfully and obtained my flag.
```
Flag:pwn.college{06DJ7Pg6psZALMbtQ0bEaH1IA8E.dFjM4QDLwEjN0czW}
```
##

## Challenge 2:Matching with ?
learned file globbing using ?. Pretty much the same thing as a * but only for a single character.

this challenge needed us to cd into challenge using ? in place of c and l,and then obtain the flag.
```
Flag:pwn.college{Yka2r26lBTOcoA6js_OvdAq7TY-.dJjM4QDLwEjN0czW}
```
##

## Challenge 3:Matching with []
learned to use file globbing using []. This is similar to ? but will search for characters mentioned in the brackets only.

This challenge had us cd into /challenge/files and then pass /challenge/run and file glob files file_a file_b file_s and file_h in one command.I used [absh] to do the same.
```
Flag:pwn.college{AeGnLFsdnTmKjdOgqNtFqa67PRV.dNjM4QDLwEjN0czW}
```
##

## Challenge 4:Matching paths with []
this challenge required the usage of [] in a file path.We had to run /challenge/run and then provide file path for files file_a file_b file_s and file_h in /challenge/files.

So I ran /challenge/run /challenge/files/file_[absh]
```
Flag:pwn.college{Yer_PHvQH5qGaxm1Hy4QnPDatYn.dRjM4QDLwEjN0czW}
```
##

## Challenge 5:Mixing globs
Had to use a mix of all the globbing methods I learned to find one generalized statement to match the files educational,pwning and challenging.

wasted a bit of time trying to find some sort of common link or pattern among the three words,unnecessary because there was no pattern and I just had to run [epc]* to get them all
```
Flag:pwn.college{0O0z4SLHmkHVS3okpd0i9wOnttD.dVjM4QDLwEjN0czW}
```
##

## Challenge 6:Exclusionary globbing
Learned that we can filter out files that we do not need using the [] method too,we just need to pass an ! or ^ at the start inside the [].

This challenge required us to filter out files starting with p,w and n in the directory. just had to pass [^pwn]* as an argument for the flag.
```
Flag:pwn.college{UelNMbNPR6p77IK2fDwKD0Hfgxp.dZjM4QDLwEjN0czW}
```
##