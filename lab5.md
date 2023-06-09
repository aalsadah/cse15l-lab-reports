# Lab Report 5

## Part 1 - Debugging Scenario

**Student:** Hello, I am working on a java program and a bash script that is supposed to take in the path of a text file and a query, and then return the line and its number of where that query appears into a new file called ```results.txt```. I am on a Windows operating software and I am using VS code for this project. Here are some screenshots of my Java program, my Bash script, and the file structure.

```LineFinder.java```
![Image](java.png)

```output.sh```

![Image](bash.png)

File structure and text files

![Image](files.png)

![Image](text.png)

![Image](words.png)

I have run into two bugs so far, the first one is that for some reason my code does not return the correct line number, I want my program to return the number of where the query appears in the original file, not in the new file. The second bug is that when I run the program a second time when it already has created a directory, I get this error message which I do not want. I hope the screenshots below demonstrates what I mean. 

First bug
![Image](bug1.png)

Second bug
![Image](bug2.png)

**TA:** Hello, thank you for sending all these screenshots, after looking at both your Java program and Bash script, I can give you some help on how to fix the bugs. For the first bug I suggest that you look at ```LineFinder.java``` and try to trace how the lines are being counted inside of the while loop, a slight fix would make sure that you would start counting the lines the way you want your program to function. The second bug has to do with the ```output.sh``` file, can you remember any command from class that removes a directory? perhaps using that command at the start of your script could solve the bug.

**Student:** Thank you for all the help I have fixed my ```LineFinder.java``` and my ```output.sh``` now the bugs I spotted are no longer there and the program is running as I intended. The line numbers are being counted properly and I am no longer getting the ```mkdir: cannot create directory ‘Search_Result’: File exists``` message. 
![Image](fix1.png)
![Image](fix2.png)
![Image](term.png)

## Part 2 - Reflection
Learning how to use Bash was extremely engaging and fun, I really liked learning how to write bash scripts and really glad this class has taught me the basics of scripting. I specifically liked learning about how you can use input/output in bash, running programms autonomously is really fun, cool, and interesting. Another thing I learned which I found really cool was how you can stop your program mid-run using Vim and check for variable or object values, I found that topic super cool, and I learning about that will come in very hand I am sure when it comes to testing and debugging my code. I also wanna say thank you to Proffesor Joe and all the amazing TA's for one of the most fun, engaging, and helpful classes I've taken all year. Thank you!


