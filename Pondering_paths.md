# Module 2: Pondering Paths

## Challenge-1:The Root
invoked the pwn program by typing in '/pwn' for the flag
```

flag:pwn.college{IltAD57FtyiyOzzudqaNLktQP6v.dhzN5QDLwEjN0czW}

```
##

## Challenge-2:Program And Absolute Paths
to access the run program in challenge in root,typed  /challenge/run and got my flag. This kind of feels like accessing the elements of a nested list in python.
```

flag:pwn.college{YvZef9ars3VKh_RcfwB38iSfJ4z.dVDN1QDLwEjN0czW}


```
##

## Challenge 3:Position Thy Self
tried running '/challenge/run' to figure out which directory to shift to,recieved output of directory name. Shifted to said directory using the 'cd' command and ran it again for the flag
```

flag:pwn.college{kK7WJ_W3FVYu3Pba8VZ9_LbC9Qp.dZDN1QDLwEjN0czW}


```
##

## Challenge 4:Position Elsewhere
same logic and process as challenge 3
```

flag:pwn.college{k-TOGJFlhkyHa1d8G9C1khNx9qo.ddDN1QDLwEjN0czW}


```
##

## Challenge 5:Position Yet Elsewhere
same logic and process as challenge 3
```

flag:pwn.college{UbytptJHm2Nw4doaYM84sAFeSsL.dhDN1QDLwEjN0czW}


```
##

## Challenge 6:Implicit Relative Paths, From /
its given that the cwd was /,so had to run 'challenge/run' for the flag because it was the relative path from '/',kind of like if we want to access an element in a nested list and the index of the sublist inside the mainlist is already given
```

flag:pwn.college{caXKbPiLoE8Fu8Gx5vMjUmETLtK.dlDN1QDLwEjN0czW}


```
##

## Challenge 7:Explicit Relative Paths, From /
switched to / directory then ran ./challenge/run for the flag because they wanted it to start with "."
```

flag:pwn.college{0HMHSgFDp6BoHU4niFXGElsuwOJ.dBTN1QDLwEjN0czW}

```
##

## Challenge 8:Implicit Relative Path
switched cd to /challenge and then to overcome the safety measure ran ./run to indicate to linux that we wanted to run 'run' from challenge only
```

flag:pwn.college{YzzGHrnOXi5bpRHJjm189EWE9-_.dFTN1QDLwEjN0czW}

```
##

## Challenge 9:Home Sweet Home
ran /challenge/run with an argument '~/a'. the ~ basically means that its referencing to the home directory meaning ~/a is now an absolute path for the file '/a'
```

flag:pwn.college{AUTfWTtWg0I2CTL-K11lmBjdvPM.dNzM4QDLwEjN0czW}

```
##
