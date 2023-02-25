# Lab Report 7
**Step 1**
_**Setup** Delete any existing forks of the repository you have on your account_

Open the repository page on github, go to the tab `Settings`, scroll down to the bottom section called `Danger zone`. Click `Delete this repository`.

![1](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-1.png?raw=true)

**Step 2**
_**Setup** Fork the repository_

Go to the github page `https://github.com/ucsd-cse15l-w23/lab7`, click `Fork` on the upper right to fork the repository.

![2](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-2.png?raw=true)

**Step 4**
_Log into ieng6_

Open VSCode. Use ``<ctrl><shift><`>`` to open a new terminal. 

Then enter `<ctrl><R>` and enter `ssh`. Bash will show my past command to log into ieng6.

![3](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-3.png?raw=true)

Press `Enter` to confirm. Now I'm logged in. Note that I have generated an SSH key and store on both my computer and the server, so I don't need to 
enter the password.

![4](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-4.png?raw=true)

**Step 5**
_Clone your fork of the repository from your Github account_

Go to the github page of my forked repository `Lab7`. Click the green button `Code`, select `SSH` and copy the link.

![5](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-5.png?raw=true)

In the terminal, enter `git clone` and then paste the link.

![6](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-6.png?raw=true)

**Step 6**
_Run the tests, demonstrating that they fail_

Enter `ls` to see the files. Enter `cd lab7`.

Again, use `<ctrl><R>` `javac` to get a record of the previously used java compile command. Press `Enter` to confirm.

Use `<ctrl><R>` `java` to get a ecord of the previously used java run command. Note that bash will still show the compile command at first. To
change it to the java run command, press `<space>`. The result is as shown. Press `<enter>` to confirm.

![7](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-7.png?raw=true)

Here we can see that one of the two tests fails.

![8](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-8.png?raw=true)

**Step 7**
_Edit the code file to fix the failing test_

First, open ListExamples.java using nano: enter `nano Li``<tab>`. Bash will autofill it to `nano ListExamples`. Then add `.java` and press `enter`.

Here we are inside nano:

![9](https://github.com/MinghanWu039/Lab-report-7/blob/main/LR7-9.png?raw=true)

Use the mouse or `down` to scroll down (we know from the error message that the problem is with the merge() method). In the third while loop
of merge(), we can see that apparently the circled `index1` should have been `index2`.

![10](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-10.png?raw=true)

Enter `<ctrl><V>` to go to the second page. Enter `<down>` until the cursor is in the same line as the error. Enter `<right>` until the cursor is right after `index1`. 

![11](https://github.com/MinghanWu039/Lab-report-7/blob/main/LR7-11.png?raw=true)

Press `<backspace>` and then enter `2`.

![12](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-12.png?raw=true)

To save and exit, press `<ctrl><o>` `<enter>` and `<ctrl><x>`.

**Step 8**  
_Run the tests, demonstrating that they now succeed_

We can now compile and run the test again, just like in step 6 (this time we can just copy and paste the commands). We can see the tests 
now both succeed.
  
![13](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-13.png?raw=true)
  
**Step 9**  
_Commit and push the resulting change to your Github account_

To apply our changes, input 

`git add .` + `<enter>`

`git commit -m "<message>"` + `<enter>`

`git push`

in that order.
  
![14](https://github.com/MinghanWu039/Lab-report-7/blob/1344344f2f36a267163f1c82b3122dba71851eda/LR7-14.png?raw=true)
  

 
