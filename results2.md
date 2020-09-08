# Results of Assignment 2

## Scores

I put the scores in an EXCEL file on Sciebo: https://th-koeln.sciebo.de/s/uP3hCLBZHagmW93

## Common mistakes

### A2E1
* Extra whitespace at start and end of chararcter names -> use trim
* unnessessary index column
* extra chars like `(` are not removed in the dataset
* wrong counts (frodo in char = 225; frodo in dialog = 149)
* Warning: Do not count the lines that mention a character but the occurrences of that character name!
* The counts for character names and dialog occurrences should not be the same!

### A2E2
* Please document how the bonus figures were generated.
* CSV2JSON needs to include readable keys that should be generated from the header 
* Just reading in the CSV file with Pandas and exporting as JSON is not enough (see previous issue)
* Missing keys and column names
* Style: Avoid filename extensions like `_final` when using version control like git.
* Using input() is considered bad style. Don't ask the user about the filename or anything else. Use parameters from the commandline.
* Style: Place imports at the beginning of the script/notebook
* If you use a source of inspriration (from the internet), please name your sources! It's no shame to read about your problem at hand and to get help - but be kind and give credit!

### A2E3
* The source list and the resulting scraping task should have something in common.
* Documentation! Please motivate what you did!
* Clean your scraped data - Sometimes you have comments within your scraped data like "Einwohnerzahl: 1432344 (Schätzung 2019)". All you want is the actual number.

