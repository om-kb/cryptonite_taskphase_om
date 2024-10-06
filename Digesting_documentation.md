# Module 4:Digesting Documentation

## Challenge 1:Learning from documentation
learned that commands must always be invoked with the right arguments specefic to the needs we have.

for this challenge I had to run /challenge/challenge with the argument --giveflag to recieve my flag
```
flag:pwn.college{82nhzF7pOTnuGrKfBwc1jcBncHl.dRjM5QDLwEjN0czW}
```
##

## Challenge 2:Learning complex usage
learned the complexity of arguments for the different comands that exists.

for this challenge i had to run /challenge/challenge with the argument --printfile again with the argument /flag to print the flag
```
flag:pwn.college{snf-Gij3vG22AcavMol7RC5Nmz9.dVjM5QDLwEjN0czW}
```
##

## Challenge 3:Reading manuals
learned a new command man. This gives us a description of any command.

for this challenge I had to use man on challenge to understand what argument to pass to get the flag. After reading the description just had to run it with the right argument.
```
flag:pwn.college{onzXdle26DEHu6YOZX-nk2pbSML.dRTM4QDLwEjN0czW}
```
##

## Challenge 4:Searching manuals 
learned a new command to pass after man produces result. The / command lets us search for whatever we want to search and can scroll up/down to the next finding using n and N 

for this challenge had to do man challenge then search for where flag was mentioned and then run the command with the right argument for the flag.
```
flag:pwn.college{0MJ9voJ-301p-XeW4Aa26pcNBoe.dVTM4QDLwEjN0czW}
```
##

## Challenge 5:Searching for manuals
learned the multiple ways of using man,This particular question required the usage of man -k .string which lets us find whatever string we are searching for. If we type in '.' before anything we type the '.'  is considered as anything.

Ran man -k .challenge which gave me the changed manpage of /challenge/challenge.

then I ran man and changed name to read challenge's man page to understand what argument to pass for the flag.
```
flag:pwn.college{M3zE_Ojxo31-Aq9YDFb2y7sppIf.dZTM4QDLwEjN0czW}
```
##

## Challenge 6:Helpful programs
Some programs don't have a manpage but we can still find out how to use the commands by passing the argument --h.

For this challenge i ran /challenge/challenge --h to find out the synopsis of the command and then used the info gained to find the flag.
```
flag:pwn.college{AhD_nHiARLRI_DWucP7u5bhrFJU.ddjM4QDLwEjN0czW}
```
##

## Challenge 7:Help for builtins
learned about what builtins are,basically the built in commands that are not user defined. Also learned how to use the help command on them, just have to type 'help cmd'.
For this challenge the challenge command was built in and so had to do help challenge to figure out how to use it and then find my flag.
```
flag:pwn.college{s0G7v-PefVdGvjrTCequhe1SeKr.dRTM5QDLwEjN0czW}
```
##