# Assignment 2 

## Exercise  0

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

## Exercise 2

### Task 1 
Write a Python program `csv2json` to convert a given CSV file into a JSON file. This conversion should be generic as possible and able to convert different types of CSV files. For the beginning try to make it work with the [`lotr_clean.csv`](lotr_clean.csv) file I uploaded to GitHub. Think about the generic parts. Where do the JSON key names come from? What about different types of separators? Try to build your program from "simple" to "a bit more complex" and think about how to split the development within your group. Document your program and remember to commit early and commit often.

### Task 2 
Your task is to transform a dataset on movies since 1950. Download the dataset [`movies.json`](movies.json) from our Github repository. Write a Python program to:

1. read in the data from the JSON file,
2. count for each year, how many movies per genre have appeared,
3. create a CSV file where for each year, the counts for each genre are listed.

Your final CSV should look something like this:

year|Action|Adventure|Animation|...
-----|------|----------|--------|---
1950|39|42|65|...
1951|...|...|...|...

### Bonus 
Create some interesting figures (in spreadsheet software, with R or any other visualitation software you know) on the development of genres over time.


## Exercise 3  

In this final assignment, we would like you to develop a little web scraping project. This is the last part of the second assignment for this semester. It includes a lot of the different tools and steps you learned during this semester.

1. Pick a list within the Wikipedia like the [list of sovereign states](https://en.wikipedia.org/wiki/List_of_sovereign_states). Choose some other list on your own, based on your personal interests. The only requirement is that there are other Wikipedia articles linked within the list.
2. Get all the names and URLs to the corresponding items in the list and export them into a CSV file that has two columns (name and URL).
3. For every Wikipedia article in the CSV list choose a few attributes from the infobox on the right that you would like to extract (e.g., population, name of the head of state, whatever...). Extract this information for every entry in your list. Store this information in an appropriate data structure.
4. Save your scraped information into a JSON file. Try to export *clean* data.
5. Document your program and development process. Tell us something about the data you scraped. Why did you choose this data? Can you think of a good use case for this data? As always: Push everything into your GitHub repository.

### Some hints

* Try to be kind to Wikipedia and yourself. You will most likely generate a lot of web traffic while scraping the same webpage again and again. This stresses the Wikipedia's server and takes a lot of time. Try to use a caching method like the one from [requests-cache](https://pypi.org/project/requests-cache/). Alternatively, you can download the HTML content using your script and then work locally.
* Try not to solve the whole problem at once. Remember the tactics desribed in the earlier lectures: [Divide and conquer](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm) - Step by step. 
* Have a look at the two sample projects from [chapter 11](https://automatetheboringstuff.com/chapter11/). They do something similar.
* A lot of code examples for Beautiful Soup are documented in the [official documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/).