# Pondering PATH

## The PATH Variable
for this challenge had to run PATH='' to blank the path.
```
flag:pwn.college{UkDnLj7BdrV4SjQhOjDTJPKEvOl.dZzNwUDLwEjN0czW}
```
##

## Setting PATH
for this challenge had to set the PATH variable to include the /challenge/more_commands/ directory and then invoked /challenge/run for the flag.
```
flag:pwn.college{gS_pRaeJy59dpgm4yzzy7YAtrHo.dVzNyUDLwEjN0czW}
```
##

## Adding Commands
for this challenge hat to create the win script and make it executable just as before,checked my current PATH variable to see the default directories using echo $PATH. Then I set the path to include the directory of the win script. Then ran /challenge/run for the flag.
```
flag:pwn.college{gS_pRaeJy59dpgm4yzzy7YAtrHo.dVzNyUDLwEjN0czW}
```
##

## Hijacking Commands
for this challenge to prevent the deletion of the flag file, had to create a custom rm script. By modifying the PATH variable, ensured that whenever we run /challenge/run, and attempt to call rm, it uses my version instead, safeguarding the flag.
```
flag:pwn.college{AIP1h81HvvZ5QzjJO0VgFFIduyQ.ddzNyUDLwEjN0czW}
```
##