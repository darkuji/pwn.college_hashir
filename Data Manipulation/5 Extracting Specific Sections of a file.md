# Extracting Specific Sections of a text
### The challenge asks us to extract specifc part of a file


## My Solve
**Flag:** pwn.college{wsS2mQsBd33484gDhY7fDfTrX60.01NxEzNxwSO1EzNzEzW}
First ran /challenge/run and saw the raw file then used cut -d " " -f 67 coz
i thought it counts characters as columns but it didn't give any output so 
instead used cut -d " " -f 2 since the p w n part was in the 2nd column and 
got the output with tr -d "\n" to remove line breaks


```
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 7 | tr -d "\n"
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{wsS2mQsBd33484gDhY7fDfTrX60.01NxEzNxwSO1EzNzEzW}
```

## What I Learned
I learned how to extract specific sections of a file

## References
None