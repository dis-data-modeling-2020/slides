# Assignment 2 

## Excercie 0

Form a team of 3-4 students. Give your team a cool name like [The Be Sharps](https://www.youtube.com/watch?v=CWbW1jtFQUo) or [The Blernsballs](https://www.youtube.com/watch?v=oQF8rQaIjUE&list=RDzfvpeVe_i1A)... You get the idea. 
When your team forming process is done, join the [GitHub Classroom](https://classroom.github.com/g/amhiWzvg) for assignment 2. Your team can then collaborate via GitHub.

## Exercise 1 

We continue with the Lord of the Rings data set and try to reproduce some of the exercises we did with shell and grep.

0. Read chapter 8 to learn more about reading and writing files. I skipped a lot of details.
1. Write a Python program that extracts a full list of all character names that are listed in column "char".
2. Extend your program to count the character names. Save the names and corresponding counts in a dictionary. 
3. Write the results in a new CSV file that contains the names and the counts. 
4. Do the same steps 1-3 again, but count the character names that appear in the column "dialog". Think about different name variations (like uppercase, etc.).

Commit your Python program and the resulting CSV files. 

## Excercise 2

### Task 1 (5 points)
Write a Python program `csv2json` to convert a given CSV file into a JSON file. This conversion should be generic as possible and able to convert different types of CSV files. For the beginning try to make it work with the [`lotr_clean.csv`](lotr_clean.csv) file I uploaded to GitHub. Think about the generic parts. Where do the JSON key names come from? What about different types of separators? Try to build your program from "simple" to "a bit more complex" and think about how to split the development within your group. Document your program and remember to commit early and commit often.

### Task 2 (6 points)
Your task is to transform a dataset on movies since 1950. Download the dataset [`movies.json`](movies.json) from our Github repository. Write a Python program to:

1. read in the data from the JSON file,
2. count for each year, how many movies per genre have appeared,
3. create a CSV file where for each year, the counts for each genre are listed.

Your final CSV should look something like this:

year|Action|Adventure|Animation|...
-----|------|----------|--------|---
1950|39|42|65|...
1951|...|...|...|...

### Bonus (up to 5 points)
Create some interesting figures (in spreadsheet software, with R or any other visualitation software you know) on the development of genres over time.
