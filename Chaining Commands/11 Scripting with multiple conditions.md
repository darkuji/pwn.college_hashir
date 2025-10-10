# Scriptng with multiple conditions
### The challenge asks us to make a script with multiple conditions


## My Solve
**Flag:** pwn.college{wywmjNorPoIK4EeXXjKId5I4WpL.0FOzMDOxwSO1EzNzEzW}
Everything same as last challenbge but added 2 extra elif blocks which print
Linux for intput learn and college for input hacker


```
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'if [ "$1" == "hack" ]' > /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'then' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo ' echo "the planet"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'elif [ "$1" == "pwn" ]' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'then' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo ' echo "college"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'elif [ "$1" == "learn" ]' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'then' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo ' echo "linux"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'else' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo ' echo "unknown"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ echo 'fi' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{wywmjNorPoIK4EeXXjKId5I4WpL.0FOzMDOxwSO1EzNzEzW}
```

## What I Learned
Learned how to add multiple conditions to a script 

## References
None