# Untangling Users

## Becoming Root With su
The su command in lets us switch to another user's account or execute commands as a different user.
for this challenge had to enter su and then cat the flag
```
Flag::pwn.college{QeBq-RwPuEW9rHdwpW8SoxDjjlI.dVTN0UDLwEjN0czW}
```
##

## Other users with su
The su command with a user as an argument allows us to switch to that user.
for this challenge i had to switch to zardus and run /challenge/run
```
flag:pwn.college{Mb-NgCw6E1-ZYGRRM7OZGwjmApB.dZTN0UDLwEjN0czW}
```
##

## Cracking passwords
found the password using /challenge/shadow-leak then did the same as challenge 2
```
flag:pwn.college{06i59404YlwGggxdVyGT4Rk1qro.ddTN0UDLwEjN0czW}
```
##

## Using sudo
sudo defaults to running a command as root.
had to pass sudo and then cat flag
```
flag:pwn.college{Y8kbrrhvJqH9p071zixLsBl8zHd.dhTN0UDLwEjN0czW}
```
##