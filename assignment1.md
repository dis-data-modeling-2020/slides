# Assignment 1

## Exercise 1 (3 points)

Create a GitHub account and join the [GitHub classroom](https://classroom.github.com/a/no15MntJ).

Once the cloning process is done create a new file in this repository via the web interface. Use `introduction.md` as file name.

Inside the file, first enter the following information:

* **Name**: {your name here}
* **E-Mail**: {your smail address here}

Then, answer the following questions:

1. Do you have any prior experience in the field introduced in the introductory session? If so, give a short overview on them.
2. What expectations or wishes do you have on the data modeling course?

Make use of some Markdown formatting like headings and lists when answering these questions, when appropriate.

Below the editor, leave the option "Commit directly to the master branch." checked and click "Commit new file".

## Exercise 2 (3 points)

### Task 1
Complete the lessons from the interactive online course at [linuxjourney.com](https://linuxjourney.com/lesson/the-shell) on learning the command line. Do the quizes in each of the lectures.

Prove your completion with a photo that shows your student ID card and the correct results of the quizes. Make at least 3 photos according to the three digits of your student ID. For example: Your student ID is 1110341 -> Photos of exercises 3, 4, and 1. In case this rule of thumd does not work, calculate the sum of the double digits or last two digits. For example: Your student ID is 1110288 -> Photos of 2, 8 and 16 (8+8). 

### Task 2
Building on exercise 1: Use your new knowledge to count the number of lines in your `introduction.md` file from exercise 1.
Redirect the result to a file, e.g. `lines.txt`.
Print the content of the file to the console.

To submit your solution, copy the commands and their outputs from the shell (including prompt) to a new *markdown-formated file* `exercise2.md`. Make use of the markdown markup for verbatim code blocks to render it nicely in monospace font.

More on markdown-formating can be found at this [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) from `adam-p` or the official [GitHub Guide to Markdown](https://guides.github.com/features/mastering-markdown/).

## Exercise 3 (5 points)

1. Clone your own repository into your local file system.
2. Play around with the [git visualization tool](https://git-school.github.io/visualizing-git/) shown in the lecture. Create some commits, branches and tags there and watch the graph grow. (Hint: typing help will show you all the available commands.)
3. Make a screenshot of your work when you’re finished. Save the screenshot on your machine to your working directory (where you cloned your repository into). Give the screenshot a reasonable filename, like `schaer-ex03.png`
4. On the command line:
  * navigate to the directory
  * check your git status
  * add the new file to git
  * and commit the change.
  * Finally, push your changes to the remote repository.
5. Visit your repository on GitHub to verify that your new file is present. 

## Exercise 4 (6 points)

Download the dataset [`shell-lesson.zip`](https://librarycarpentry.org/lc-shell/data/shell-lesson.zip) from the previous lecture 02 and unzip it.

Write a set of shell commands to do the following things:

1. Print an overview of the number of lines per `.tsv` file on the occurence of the terms `china` or `chinese`.
2. Do the same, but search only in the title column. _Hint: Make use of the `cut` command._
3. Count the number of lines that contain an ISSN in all `.tsv` files. _Hint: Check on the correct pattern with `grep`._
4. Print an overview of all entries on creators in the `.tsv` files.
5. Print an overview of unique creator names in all `.tsv` files. _Hint: Make use of the `uniq` command._
6. Print an overview of the ISSN numbers, sort them, delete duplicates and save the result to a file named `uniq-issn.txt`.

### Submission instructions for Exercise 4

Create a file `exercise04.sh` that will contain your solutions to the 6 tasks.

* First line has to be `#!/bin/bash`
* Each line contains the command to solve one of the tasks above.
* We want to see one commit in GitHub per solution!

Additionally, create a text file `exercise04.md` and comment on each solution. To do that,

* copy your commands into the Markdown file,
* and explain what you did and why.

Push all commits to your repository.

## Exercise 5 (8 points)

In this exercise, you will be working with the dataset [`lotr_scripts.csv`](lotr_scripts.csv). The original data set can be found on [Kaggle](https://www.kaggle.com/paultimothymooney/lord-of-the-rings-data). 

1. Document the different data fields. (1 point)
2. Identify "dirty" data fields and clean them up. Use regex replace, spreadsheets or whatever you like. Document your working steps in a file `exercise05.md`. Export your data set as a clean CSV file. Add both files to your repository. (5 points)
3. Analyze the data set using shell scripts and/or regex. Document the commands in an additional section in `exercise05.md`. (2 points)
    * Find the total number of lines and unique words used in the dialogs. (0.5p)
    * What is the distribution on the three different films? (0.5p)
    * What are the top 5 characters in the char column? (0.5p)
    * What are the top 5 characters in the dialogs? (0.5p)

Documentation is key! Everything that is **not properly documented** is not verifyable by us and will thus get **0 points**.
