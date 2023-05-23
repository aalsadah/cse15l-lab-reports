# Lab 4: Using ```vim``` and git commands

**Step 4:** I first logged into my ieng6 account using the ```ssh``` command

**Step 5:** I then cloned the git repository using the following command: ``` git clone https://github.com/ucsd-cse15l-s23/lab7```

**Step 6:** I type ```bash test.sh``` to run the tests and demonstrates that they fail. 

**Step 7:** I type the command ```vim ListExamples.java``` so that I can edit the bugged java file. I pressed the ```<J>``` key 43 times, and the ```<L>``` key 2 times to navigate to where the error was. I am now at the start of the word ```index1```, so now I type the command ```dw``` to delete that word and then I press the key ```<I>``` to enter insert mode. Once in insert mode I type the correct code which is ```index2```, I then press the ```<esc>``` key to return to normal mode. I then type ```:wq``` to exit and save the file. 

**Step 8:** I type in the command ```bash test.sh``` to test the file, the tests succeed. 

**Step 9:** Finally I type the command ``` git add ListExamples.java```  then the command ```git commit``` to commit my changes and then I log out of ieng6 using ```exit```. 
