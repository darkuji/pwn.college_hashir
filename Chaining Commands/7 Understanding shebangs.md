# Understanding shebangs
### The challenge asks us to use shebangs to execute a script


## My Solve
**Flag:** pwn.college{QzJLYN6e-a1eapp6Yc2tMw8CsWx.0VOzMDOxwSO1EzNzEzW}
Used echo '#!/bin/bash' > /home/hacker/solve.sh to move it to the script
as it is a shebang then used  echo 'echo "hack the planet"' >> /home/hacker/solve.sh
to move it to the script which is the actual content of the script then used 
chmod a+x /home/hacker/solve.sh to make it executable and ran /challenge/run


```
hacker@chaining~understanding-shebangs:~$ chmod a+x /home/hacker/solve.sh
chmod: cannot access '/home/hacker/solve.sh': No such file or directory
hacker@chaining~understanding-shebangs:~$ echo '#!/bin/bash' > /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ echo 'echo "hack the planet"' >> /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ chmod a+x /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{QzJLYN6e-a1eapp6Yc2tMw8CsWx.0VOzMDOxwSO1EzNzEzW}
```

## What I Learned
I learned how the Linux compiler often sees the starting content of a file to know its types
which are also called shebangs and how to add one to your script

## References
None