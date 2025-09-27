# Matching paths with []
### The challenge asks us to search for files in a different directory []


## My Solve
**Flag:** pwn.college{4D26k6La_jw83fOLFNyJnMhfX7e.QX0IDO0wSO1EzNzEzW}
I used the argument /challenge/files as that was the path of the files
and gave the files_[bash] argument to search for files b a s and h


```
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{4D26k6La_jw83fOLFNyJnMhfX7e.QX0IDO0wSO1EzNzEzW}
```

## What I Learned
I learned how we can also search for files with [] if we 
are in a different directory

## References
None