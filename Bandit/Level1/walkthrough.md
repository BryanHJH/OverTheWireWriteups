# Bandit: Level 1 

## Getting into Level 1

This level is also considered easy for a computer science major. 

In this level, they require us to read the contents of a file in the home directory. 

Normally, the first thing you would do is to check where you currently are using the `pwd` command, but I skipped this step. 

What I did was just immediately use `ls` to list out all the contents of the current directory, which immediately showed the file I needed. 

Then, I just used `cat FILENAME` to display the contents of the identified file. And there you have it, the password required to SSH into the next level. So to SSH into the next level, we just use the SSH command from Level0.

## Getting out of Level 1

To get out Level 1, we again need to find the password for the next level. This time, again, the file is located in the home directory. However, this time the file is named "-", just a dash. 

After quickly googling around, I found that the command required to read the contents of the file is to just do `cat ./-` and voila, the password is shown to you. 
