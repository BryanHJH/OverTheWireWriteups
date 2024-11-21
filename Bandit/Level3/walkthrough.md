# Bandit: Level 3

## Getting out of Level 3

Again, getting the password to enter Level 3 is already written in Level 2's walkthrough. 

SO now, the password for the next level is actually in another directory and to get into the other directory the command `cd` is used. The usage is like this `cd DIRECTORY` where DIRECTORY is the folder or directory that you want to go into. 

Once in the next directory, if you run `ls` to list out the contents of the directory,  you will see nothing, this is because the file we're looking for is a hidden file (basically files that start with a dot(.) in their filenames). To display such files when listing the contents of a directory, we need to run `ls -l` or `ll`. Once we have the filename, we can either use the method in Level1 or Level2 to see the password.  
