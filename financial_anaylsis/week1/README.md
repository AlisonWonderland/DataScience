# Week 1 

Repo where I store files from this coursera course: https://www.coursera.org/learn/python-statistics-financial-analysis/

Will be using these files as reference for later work

## What I learned from this week
*  I learned about functions/methods that are used to obtain and print a certain number of rows from our DataFrame object.
* Learned that you can index a DataFrame column using dfName['column']. Useful when you only want the rows from that column by combining with the loc() or iloc methods
* You can create a new column for the DataFrame by doing dfName['new column name'] = something.
* List comprehension. Which is a way of adding items to a list in python. Syntax in the notebook is different than examples that I've found online. Looks familiar to the ternary operator from C.
* Shift() by default positive number moves columns down. Negative moves them up.
* Rolling() is used to collect a certain number of rows in our DF, whether it'd it be the entire DF or a column, and perform an operation on those rows. The number of rows is called the window. Rolling() on its own doesn't do anything. rolling() must be followed by an operation function. For example: ex['Previous 50 prices summed'] = ex['Price'].rolling(50).sum() or ex.rolling(50).sum()
In the first example, a new column will be created with the sum of the 50 previous prices. Meaning that if a row doesn't have 50 rows before it then the sum will show up as NaN
* dropna() Remove rows that are missing a cell of data.
* cumsum() To sum up all the values in a column.
