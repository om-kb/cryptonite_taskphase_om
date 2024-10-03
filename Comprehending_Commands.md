# Module 3:Comprehending Commands

## Challenge 1:Cat: not the pet, but the command
learned a new command called cat,it reads any file provided as an argument. 

This challenge required us to read a file called flag placed in the home directory so ran 'cat flag' for the flag.
```
flag:pwn.college{k5I6mF8I1_CvuhI1--ZCfPfY8WQ.dFzN1QDLwEjN0czW}
```
##

## Challenge 2:Catting absolute paths
used cat on the absolute path of flag which was '/flag'
```
flag:pwn.college{8hdJv72vlh-qUM4w3GGy7_9-y0j.dlTM5QDLwEjN0czW}
```
##

## Challenge 3:More catting practice
ran the cat command with the directory given 
```
flag:pwn.college{cxnPkDevO2Ow7bbPCEqSjFAczLw.dBjM5QDLwEjN0czW}
```
##

## Challenge 4:Grepping for a needle in a haystack
learned a new command called grep. It finds any line in a file and reads it,the line to be found must start with whatever argument we pass in the grep command.

for this,we know all flags start with pwn.college so I ran grep with that argument and mentioned the path given.
```
flag:pwn.college{QcteEkVrX1jgViCncYaJgsIAtYf.ddTM4QDLwEjN0czW}
```
##

## Challenge 5:Listing files
learned new command ls. It basically just lists out all the files in a directory.

for this challenge we needed to find out what run was renamed to,which I did by listing out all the files in /challenge and then just catting the path.
```
flag:pwn.college{UoEhgFzULN7gXaPza4c79uvyWo1.dhjM4QDLwEjN0czW}
```
##

## Challenge 6:Touching files
learned a new command again called touch. This lets us create any new files in our cwd.

this challenge required us to create two files pwn and college in a directory called tmp so I cd into tmp and touched twice then did 'cd ..' to get back to my home directory and ran /challenge/run for my flag
```
flag:pwn.college{g6ZfhS7umcJp4VprrarPiFxbTkn.dBzM4QDLwEjN0czW}
```
##

## Challenge 7:Removing files
learned another command called 'rm' used to delete any file in cwd.

this challenge needed us to create and delete a file in the home directory so used touch and rm and then ran /challenge/check for my flag
```
flag:pwn.college{wF3JVMS7-_9-DYNCSRkTGHEJv-t.dZTOwUDLwEjN0czW}
```
##

## Challenge 8:Hidden files
learned that ls does not show the files that start with a '.', to make it show them too we need to pass an argument -a with ls.

This challenge needed us to find the name of the file with the flag which started with a . so switched cwd to / and ran ls -a to see all the files,identified and ran the cat command with the flag file.
```
flag:pwn.college{8DOsWatYmGr-f8MR5gvyZUE2zXN.dBTN4QDLwEjN0czW}
```
##

## Challenge 9:An epic filesystem quest
lot of finding clues and following a trail of breadcrumbs in this challenge. Utilized ls and cat for this challenge while seeing the files of all the directories and then reading the clues.
```
flag:pwn.college{05GtgcqzO_UN3lLXtlWEs25sTVG.dljM4QDLwEjN0czW}
```
##

## Challenge 10:Making directories
learned a new command 'mkdir'. This makes a new directory where we can create and store files.

This challenge required us to make a new directory using mkdir, then add a file using touch and finally running /challenge/run for the flag.
```
flag:pwn.college{ocVPD0pKjg4BmEr1NMNpEtCvjzU.dFzM4QDLwEjN0czW}
```
##

## Challenge 11:Finding files
learned a new command 'find' which finds whatever we want to search for. We can specify the name and search location of whatever we are searching for.

for this challenge we needed to find 'flag' so I used find and specified the name flag to find the flag and then read it
```
flag:pwn.college{Y2GlEs0GzKPtZtBf3RCh1LIrGP_.dJzM4QDLwEjN0czW}
```
##

## Challenge 12:Linking files
understood the concept of linking files,how there are two types hard(2 names for same thing) and soft(forwarding it from one name to other).

also learned a new command,the command for soft linking is ls with the argument -s then pass the original file and then the file we would like to serve as a pointer to the original.

also learned a new comand file,this tells us the type of file the file passed as an argument is.

for this challenge we had to make /home/hacker/not-the-flag point to /flag so I ran 'ls -s /flag /home/hacker/not-the-flag' and '/challenge/catflag' for my flag
```
flag:pwn.college{EvMnwlFNNHb0tD2CFkYoMMHp7Fl.dlTM1UDLwEjN0czW}
```
##
