# Hints for Exercise 5

## Part 1 - Reading and dividing the data file
1. **Extracting the year for each line of the data file**.
In order to isolate the year when processing the data in the data file for this exercise, you need to use a substring, or part of a character string, from the values in column 6 of the `816295.csv` data file.
Those values have the form `YYYYMMDD` where `YYYY` is the year of the observation, `MM` is the month, and `DD` is the day.
You want to use only the year, and let's assume that for each line of the data file that is read, you assign the value in column 6 to a variable `date`.
The year part of `date` would then just be the first 4 characters in `date`, and since character strings are simply a list of characters, you can use the index values to extract a slice (or substring) from the variable `date`.
Since the first number in the year in `date` would simply be `date[0]`, and the last would be `date[3]`, all we need is a way to use only index values 0-3 in date.
You can access a range of index values in a string variable or list using the colon (`:`) character.
The example below may help make things more clear:

    ```python
    >>> text = "Helsinki"
    >>> print(text[0])
    'H'
    >>> print(text[3])
    's'
    >>> print(text[0:3]
    'Hel'
    ```
**Note**: Like the `range()` function, the last index value given in a range of values is not included in the list of indices.

## Part 2 - Calculating annual summer and winter temperatures

## Part 3 - Saving your seasonal average files to GitHub
