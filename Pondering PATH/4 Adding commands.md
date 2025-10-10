# Adding commands
### The challenge asks us to add our own commands


## My Solve
**Flag:** pwn.college{0-2iy9QYOwLCn-yQY9C1HXUX8RW.QX2cjM1wSO1EzNzEzW}
First created myscripts directory to put win using mkdir and changed cwd using cd
then created win file and put in the command required into it then
made it so that all users could execute the win command then set 
PATH to the directory with win and ran /challenge/run


```
hacker@path~adding-commands:~$ mkdir ~/myscripts
hacker@path~adding-commands:~$ cd ~/myscripts
hacker@path~adding-commands:~/myscripts$ echo '/run/dojo/bin/cat /flag' > win
hacker@path~adding-commands:~/myscripts$ chmod a+x win
hacker@path~adding-commands:~/myscripts$ PATH=~/myscripts
hacker@path~adding-commands:~/myscripts$ /challenge/run
Invoking 'win'....
pwn.college{0-2iy9QYOwLCn-yQY9C1HXUX8RW.QX2cjM1wSO1EzNzEzW}
```

## What I Learned
I learned how to add new commands using PATH

## References
None