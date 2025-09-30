# Exporting Variables
### The challenge asks us to export local variables to the main shell


## My Solve
**Flag:** pwn.college{oySbNI_PG-1277IpCi_8jK_GdUx.QXyYTN0wSO1EzNzEzW}
Assigned the required values of PWN and COLLEGE and exported PWN before
changing to sh and running /challenge/run


```
hacker@variables~exporting-variables:~$ PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ sh
sh-5.2$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{oySbNI_PG-1277IpCi_8jK_GdUx.QXyYTN0wSO1EzNzEzW}
```

## What I Learned
Learned how local variables can be exported to the shell memory

## References
None