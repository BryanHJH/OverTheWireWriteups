# Bandit: Level 4

## Getting out of Level 4

So, same thing as Level 3, first we go into the `inhere` directory using `cd inhere/`.  

Then once we're inside the directory, we'll see a bunch of files name `-file0X` where X is a number from 0-9.

So, if we look into the contents of the file using `cat`, it will just be a bunch of gibberish. When this happens, the command to use is `strings`. This would "convert" all those gibberish into human-readable text, but there are still a lot of files and I'm lazy to do it one by one. 

So here's my final command: `strings ./-file0*`, the asterisk is a wildcard replacing the wildcard with any characters, so this command in the end will apply strings on all the files in the `inhere` directory. And we will get the password!
