# Lab Report 7
**Step 1**
_**Setup** Delete any existing forks of the repository you have on your account_

Open the repository page on github, go to the tab `Settings`, scroll down to the bottom section called `Danger zone`. Click `Delete this repository`.

**Step 2**
_**Setup** Fork the repository_

Go to the github page `https://github.com/ucsd-cse15l-w23/lab7`, click `Fork` on the upper right to fork the repository.

**Step 4**
_Log into ieng6_

Open VSCode. Use ``<ctrl><shift><`>`` to open a new terminal. 

Then enter `<ctrl><R>` and enter `ssh`. Bash will show my past command to log into ieng6.

Press `Enter` to confirm. Now I'm logged in. Note that I have generated an SSH key and store on both my computer and the server, so I don't need to 
enter the password.

**Step 5**
_Clone your fork of the repository from your Github account_

Go to the github page of my forked repository `Lab7`. Click the green button `Code`, select `SSH` and copy the link.

In the terminal, enter `git clone` and then paste the link.

**Step 6**
_Run the tests, demonstrating that they fail_

Enter `ls` to see the files. Enter `cd lab7`.

Again, use `<ctrl><R>` `javac` to get a record of the previously used java compile command. Press `Enter` to confirm.

Use `<ctrl><R>` `java` to get a ecord of the previously used java run command. Note that bash will still show the compile command at first. To
change it to the java run command, press `<space>`. The result is as shown. Press `<enter>` to confirm.

Here we can see that one of the two tests fails.

**Step 7**
_Edit the code file to fix the failing test_

First, open ListExamples.java using nano: enter `nano Li``<tab>`. Bash will autofill it to `nano ListExamples`. Then add `.java` and press `enter`.

Here we are inside nano:

Use the mouse or `down` to scroll down (we know from the error message that the problem is with the merge() method). In the third while loop
of merge(), we can see that apparently the circled `index1` should have been `index2`.

Enter `<down>` until the cursor is in the same line as the error. Enter `<right>` until the cursor is right after `index1`. Press `<backspace>` 
and then enter `2`.

To save and exit, press `<ctrl><o>` `<enter>` and <ctrl><x>`.

**Step 8**  
_Run the tests, demonstrating that they now succeed_

We can now compile and run the test again, just like in step 6 (this time we can just copy and paste the commands). We can see the tests 
now both succeed.
  
**Step 9**  
_Commit and push the resulting change to your Github account_

To apply our changes, input 

`git add .` + `<enter>`

`git commit -m "<message>"` + `<enter>`

`git push`

in that order.
  

 
