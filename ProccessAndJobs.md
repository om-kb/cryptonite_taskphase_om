# Proccess And Jobs

## Listing Processes

Used ps aux and then ran the required command.
```
Flag:pwn.college{cKl8Q4EryiAVvar4Db7ViPOhxCi.dhzM4QDLwEjN0czW}
```
##


## Killing processes

To terminate /challenge/dont_run so that /challenge/run could execute, I first found its PID using ps -e | grep /challenge/dont_run, which returned 73. I then executed kill 73 to stop the process, followed by running /challenge/run to retrieve the flag.
```
Flag:pwn.college{QZNk6K7YmSAetXtSk0LncZVbNhZ.dJDN4QDLwEjN0czW}
```
##


## Interrupting processes

Ran challenge/run and used ctrl+c to interrupt it.
```
Flag:pwn.college{oEhDUcqVkGb7vCUhkHRa6ENi5PI.dNDN4QDLwEjN0czW}
```
##


## Suspending Processes

Ran challenge/run, then ctrl+z then ran the command again after which I retrieved the flag.
```
Flag:pwn.college{ICvI0dL_xVWfRB31ikztR0qT_sK.dVDN4QDLwEjN0czW}
```
##


## Resuming Processes

Ran challenge/run, then ctrl+z then ran the command fg /challenge/run after which I retrieved the flag.
```
Flag:pwn.college{EmWGjCklHNPo9CuWeOS-o1cP9qV.dZDN4QDLwEjN0czW}
```
##


## Backgrounding Processes

Similar to before, I used bg /challenge/run, after which I ran /challenge/run again.
```
Flag:pwn.college{8g6jjxmI6rgdPe_bZND0XP30dYq.ddDN4QDLwEjN0czW}
```
##


## Foregrounding Processes

This challenge involved first suspending /challenge/run using Ctrl-Z, then resuming it in the background with bg /challenge/run, and finally bringing it back to the foreground using fg /challenge/run.
```
Flag:pwn.college{M4_1bU329UNnERE-Q9K-A8mYKvd.dhDN4QDLwEjN0czW}
```
##


## Starting background processes

To run /challenge/run in the background and retrieve the flag, I simply executed /challenge/run &.
```
FLag:pwn.college{YBu81M9vOri84GWsc2z5uysMpiY.dlDN4QDLwEjN0czW}
```
##


## Process Exit Codes

To obtain the exit code of /challenge/get-code, I executed it, and it terminated with an error code. I then ran echo $?, which returned 236. Subsequently, I passed this code as an argument to /challenge/submit-code 236 and successfully retrieved the flag.
```
Flag:pwn.college{8MMcR1vR16y_yqDFgDNYCSqCuGN.dljN4UDLwEjN0czW}
```
##