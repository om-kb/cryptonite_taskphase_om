# Module 6:Practicing Piping

## Challenge 1:Redirecting Output
Learned how to redirect output to any file using >. The syntax is output > file.

For this challenge had to redirect PWN to COLLEGE fr flag so did echo PWN > COLLEGE
```
flag:pwn.college{od94xTT3KHVBRuRn_fED_KqSEpU.dRjN1QDLwEjN0czW}
```
##

## Challenge 2:Redirecting More Output
used > to redirect output of /challenge/run to myflag then read it for the flag
```
flag:pwn.college{AxuwHw24US93txujDK_zymgCLRA.dVjN1QDLwEjN0czW}
```
##

## Challenge 3:Appending Output
Learned that > makes a new file everytime we use it,deleting the contents of whatever was in it before(kind of like the write mode in text files on python)

To overcome this we use the >> command which does not overwrite the file but simply adds on to it(kind of like the append mode in text files on python)

In this challenge the flag was divided into 2 parts so we had to append it to the file instead of truncating and then read it.
```
flag:pwn.college{YS4YHZBP3KY1fgkERZuMMgJz_vj.ddDM5QDLwEjN0czW}
```
##

## Challenge 4:Redirrecting Errors
Learned about File Descriptor numbers. A File Descriptor (FD) is a number the describes a communication channel in Linux.0-input 1-output 2-error.

So to  redirect errors we just use 2> or 2>>.

This challenge needed us to redirect the output and error to myflag and instructions. Then I read the myflag file for my flag.
```
flag:pwn.college{IX0G_XA5H9IKVuzSJFhzWVbYCpr.ddjN1QDLwEjN0czW}
```
##

## Challenge 5:Redirecting Input
Learned the command for input redirection, the opposite of output redirection actually, <.

This challenge required me to first redirect the output of echo COLLEGE into PWN and then the input of PWN to /challenge/run for the flag
```
flag:pwn.college{QmsUawfVpdyI82fSdtTXjDfixFX.dBzN1QDLwEjN0czW}
```
##

## Challenge 6:Grepping Stored Results
Shifted the output of /challenge/run to a file andthen used grep pwn.college for the flag
```
flag:pwn.college{EGVg375gqHe08TqZcQDMY5UjKX3.dhTM4QDLwEjN0czW}
```
##

## Challenge 7:Grepping Live Output
We learned a new command | which basically erradicates the need to store output in a file. We just run the command | grep whatever we need.

In this challenge i ran /challenge/run | grep pwn.college for my flag
```
flag:pwn.college{ADcWb__hmyxSMm46XNHYOUODYRm.dlTM4QDLwEjN0czW}
```
##

## Challenge 8:Grepping Errors
We can not use 2| to grep errors.

The shell has a >& operator, which redirects a file descriptor to another file descriptor. 
This means that we can have a two-step process to grep through errors: 

first, we redirect standard error to standard output (2>& 1) .

then pipe the now-combined stderr and stdout as normal (|)!

For this challenge ran /challenge/run 2>& 1 | grep pwn.college to first coonvert error to output and then grep the flag.
```
flag:pwn.college{IM8L6o7Xg4b4k6gRJyFfwSnvOYW.dVDM5QDLwEjN0czW}
```
##

## Challenge 9:Duplicating piped data with tee 
The | command doesn't store the output anywhere but it will do so if passed with tee.

For this challenge i had to run /challenge/pwn | tee ab | /challenge/college and then read ab for the code and then run /challenge/pwn --secret UjM9G0d_ | /challenge/college for the flag.
```
flag:pwn.college{UjM9G0d_S-irUXeOvkLPUinNGft.dFjM5QDLwEjN0czW}
```
##

## Challenge 10:Writing To Multiple Programs
If you write an argument of >(rev), bash will run the rev command (this command reads data from standard input, reverses its order, and writes it to standard output!), but hook up its input to a temporary file that it will create.(referenced from the challenge description itself)

For this challenge I had to take output of /challenge/hack and pass it as input to the files /challenge/the and /challenge/planet files by running /challenge/hack | tee >( /challenge/the ) >( /challenge/planet )
```
flag:pwn.college{UAMFYENhgwOm-aWTo0mJzhaSrgy.dBDO0UDLwEjN0czW}
```
##

## Challenge 11:Slit-piping stderr and stdout
For this challenge i had to connect the output of /challenge/hack to /challenge/input and the errors to /challenge/the using process substitution
```
flag:pwn.college{Y13GNYZ47OpfdlShL8kqcokAt94.dFDNwYDLwEjN0czW}
```
##