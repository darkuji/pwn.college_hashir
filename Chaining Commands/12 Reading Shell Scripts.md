# Reading Shell Scripts
### The challenge asks us to read a shell script


## My Solve
**Flag:** pwn.college{M2taLdY5kZ2JLGgzx78ZJWdOQLq.0lMwgDOxwSO1EzNzEzW}
Used cat /challenge/run to read the script then figured out that i 
need to run /challenge/run and put password as hack the PLANET to get 
the flag


```
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{M2taLdY5kZ2JLGgzx78ZJWdOQLq.0lMwgDOxwSO1EzNzEzW}

```

## What I Learned
Learned how to read a script 

## References
None