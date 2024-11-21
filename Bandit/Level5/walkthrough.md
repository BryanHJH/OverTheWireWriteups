# Bandit: Level 5

## Getting out of Level 5

So, this level became much more trickier, though not much of a challenge for someone who knows their linux commands. This is my way of doing it but I'm very certain there are better and more elegant solutions out there. So let's begin. 

Same idea, first thing I did was jumped into `inhere` and once in there, I was shocked to see much more folders in there. I am not going to go in one-by-one to try and find the password, so what I did was to recursively scan for subdirectories and list out all the contents of those identified subdirectories. The command to do this is: `ls -R DIRECTORY`, which did the trick! It listed the contents of the subdirectories I saw when I first jumped into `inhere`. 

Bad news is, there are also tons of files. I went to look at the contents for a few files and all of them are similar, all possibly storing the passwords. If one have a lot of time to waste, they can try one-by-one to find the correct password, but let's use the tips OverTheWire gave, which are:

1. human-readable
2. 1033 bytes in size
3. not executable

So give these tips, we know the type of file (from no. 3) and the size of the file (from no. 2). From here, we know we need to look at the size and type of file, and `ls` has a useful flag that allows us to do just that, and it was used previously n Level 4, the `-l` flag. So combining all flags, our command now becomes `ls -lR` but going through the list, it doesn't see that there are any files that have 1033 bytes. Maybe I'm missing something. 

There might be hidden files, after all, one of the previous Levels had us finding for hidden files, so adding `-a` into the current list of flags, we have `ls -lRa`. Going through this new list, the file storing the password we want can be found, just need to look through the entire list.  
