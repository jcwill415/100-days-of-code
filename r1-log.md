# #100DaysOfCode Log - Round 1 - [Jenna Williams]

The log of my #100DaysOfCode challenge. Started on [June 16, Sunday, 2019].

## Log

### R1D1 6/16/19
Worked on CSS Basics @treehouse. Basic selectors, common values & units. https://teamtreehouse.com/ 4hrs prework @codelouisville.

### R1D2 6/17/19
AM tutorials #Python #AutomateTheBoringStuffWithPython. CSS text/box shadows & gradients @treehouse. 2hrs prework @codelouisville.

### R1D3 6/18/19
Completed @codelouisville pre-work: #HTML and #CSS. Reviewing a @treehouse #SQL course. Having so much fun! We use a relational database at work using SQL, and I'm excited to improve my #SQL skills and put them to good use. Plan to review some practice exercises in #HTML and #CSS before 6/26.

### R1D4 6/19/19
Still reviewing #SQL @treehouse! w3schools.com/sql/sql_select.asp

Write SELECT statement to query data from relational database
Select specific columns
Searching tables using 'WHERE'
Filter by comparing values

### R1D5 06/20/19
R1D5: Made progress in @treehouse #SQL course, reviewing relational operators. Having fun! Working on basics, then focus on writing better queries.

Also looking at @thew3cx courses on http://edx.org  #HTML5 & #JavaScript soon!

### R1D6 06/21/19
Modifying #SQL @treehouse, review & practice. Practice, practice, practice. 

5hrs to go in SQL Basics -- learning a lot everyday!

### R1D7 06/22/19
@treehouse + modifying data w/ #SQL. Updating Data in a Database badge.

### R1D8 06/23/19
R1D8: Reporting w/ #SQL @treehouse. Working on data handling - ordering, limiting, manipulating text, and aggregation.

SQL Basics Cheatsheet:
https://github.com/treehouse/cheatsheets/blob/master/sql_basics/cheatsheet.md

Reporting w/ SQL Cheatsheet: https://github.com/treehouse/cheatsheets/blob/master/reporting_with_sql/cheatsheet.md

Reporting w/ #SQL @treehouse part 2. Ordering Limiting. Paging Results.

### R1D9 06/24/19
Reporting w/ #SQL @treehouse; Functions/CONCAT. About an hr left on this module!

### R1D10 06/25/19
SQL @treehouse - completed 1 hr during lunch!

aggregate & numeric functions
moving on to differences b/w databases...after work!

### R1D11 06/26/19 - part 2
1. What will the following function return?
DATE("2016-02-10 22:21:23", "+1 year")
"2017-02-10"

2. Counting all values in a specific column will count all rows including empty or NULL values.
FALSE

3. What function would I use to get the average of numeric values in a column?
AVG();

4. The - is a(n): Operator

5. Which of the following is the correct way to use the STRFTIME() function?
A	STRFTIME("3118-12-01", "+3 years", "%Y-%m-%d")
B	STRFTIME("3118-12-01", "%Y-%m-%d", "+3 years")
C	STRFTIME("%Y-%m-%d", "3118-12-01") - correct

6. The ___ function is used to make strings uppercase.
UPPER

7. What will this date and modifier produce?
DATE("now", "+1 day")
Tommorrow

8. LENGTH() is described as a: Function

9. The ___ keyword is used after the ORDER BY clause to order dates from the most recent to the furthest back in time.
DESC

10. _____ BY is used to aggregate rows together.
GROUP

11. If today was the 8th July 2018, how would I write that date in SQLite/SQL Playground?
"2018-07-08"

12. ___ is the operator you'd use to add two pieces of text together in SQLite/SQL Playground.
||
CONCAT

13. What is the correct way of using the REPLACE() function for replacing "javascript" with "JavaScript"?

SELECT REPLACE("I can't capitalize javascript correctly!", "JavaScript",
"javascript");

14. ____ is a keyword that can be used in conjunction with LIMIT to page through results. 
OFFSET

15. What will this function return?
TIME("2016-10-11 23:59:00", "+2 minutes")
"00:01:00"

DATE() Function  
DATE("now") - get today's date w/ time string "now"
DATE("2016-12-19 09:10:55") - trim off time portion of time string
DATE("2016-12-19 09:10:55", "+1 year") - w/ modifier to calculate dates too

TIME() Function
TIME("now") - get time "now"
TIME("2016-12-19 09:10:55") - remove date from time string
TIME("2016-12-19 09:10:55", "+1 hour") - w/ modifier to create new date strings

STRFTIME() Function
Format with values substituted by parts of the date passed in the second argument of the STRFTIME Function

STRFTIME("%d-%-m", "now")
STRFTIME("%m-%-Y", "2016-12-19 09:10:55")
STRFTIME("%Y", "2016-12-19 09:10:55", "+1 year")

### R1D11 06/26/19 - part 1
In a movies database we have a movies table. It has the columns of id, title, date_released and genre.

Write a query that returns the title first and the month and year it was released alias as month_year_released. Dates should look like "04/1983" for April 1983.

SELECT title, STRFTIME("%m/%Y", date_released) AS month_year_released FROM movies;

STRFTIME()
STRFTIME(<format string>, <time string>, <modifier>)
            -> "01/04/2015"
STRFTIME(<format string>, "2015-04-01 23:12:01", <modifier>)

STRFTIME("%d%m$Y", "2015-04-01 23:12:01", <modifier>)
            -> "01/04/2015"

SELECT *, ordered_on AS UK_date FROM orders;
SELECT *, STRFTIME("%d%m%Y", ordered_on) AS UK_date FROM orders;

Formatting Dates For Reporting
The dates stored in a database often don't suit a human reader. 

Documentation Links for Formatting Dates

SQLite - https://www.sqlite.org/lang_datefunc.html
MS SQL - https://docs.microsoft.com/en-us/sql/t-sql/functions/date-and-time-data-types-and-functions-transact-sql?view=sql-server-2017#SetorGetSessionFormatFunctions
PostgreSQL - https://www.postgresql.org/docs/9.1/functions-datetime.html
MySQL - https://dev.mysql.com/doc/refman/5.5/en/date-and-time-functions.html
Oracle -https://docs.oracle.com/cd/B28359_01/server.111/b28286/sql_elements004.htm

Cheat Sheets
SQL Basics - https://github.com/treehouse/cheatsheets/blob/master/sql_basics/cheatsheet.md
Reporting with SQL - https://github.com/treehouse/cheatsheets/blob/master/reporting_with_sql/cheatsheet.md

-- DATE(<time string>, <modifiers>)

SELECT COUNT(*) FROM orders WHERE ordered_on
BETWEEN DATE("now", "-7 days") AND DATE("now", "-1 day");

SELECT COUNT(*) FROM orders WHERE ordered_on
BETWEEN DATE("now", "-7 days", "-7 days")
    AND DATE("now", "-1 day", "-7 days");

### R1D12 06/27/19
Downloaded anaconda for Python 3.7 & Jupyter Notebooks. Very excited. Also checking out the GitHub Guides! #HelloWorld

Completed Reporting w/ SQL: SQL can be used to generate reports and present information on websites.

Finishing Querying Relational Databases - 98 minutes left.

Inner Joins
Inner Joins are the most common types of Joins. Inner joins match records together where values are equal on both sides of the join statement.

-- SELECT <columns> FROM <table1> INNER JOIN <table2> ON <equality criteria> WHERE <search criteria> ...

-- What are all Chevy models?

SELECT * FROM make INNER JOIN model ON make.MakeID = model.MakeID;

SELECT MakeName, ModelName FROM make
  INNER JOIN model ON make.MakeID = model.MakeID;
  
SELECT MakeName, ModelName FROM make AS mk
  INNER JOIN model AS md ON mk.MakeID = md.MakeID;

### R1D13 06/28/19
Working on @udemy Automate the Boring Stuff w/ #python!

Installed @anacondainc and checking out @ProjectJupyter. 🤩💻📚

Narsingani Amisha
@amisha7069
Replying to @jcwill415 @Anansi_girrl and 3 others
Try this, it's helpful.

@AlSweigart

38,000 people have signed up for my Automate the Boring Stuff with Python online course so far. It's free for two days with this link:

### R1D14 06/29/19
R1D14: Helped a friend with their CIT capstone project and portfolio @wordpressdotcom.

Reviewed some #HTML and #CSS. Still working on my @github.

Coffee. Coding. Fun day! ☕💻🤩

### R1D15 06/30/19
Worked on my RDBMS course online...

### R1D15 07/01/19
Worked on my RDBMS course online...

### R1D15 07/02/19
Still helping a friend w/ @wordpressdotcom for their CIT capstone!

Working on week 1 review #python🐍 @MITxonedX. Finished the first week of assignments for my DBMS course. 🤩

### R1D16 07/03/19
Still helping a friend w/ @wordpressdotcom for their CIT capstone!

Working on week 1 review #python🐍 @MITxonedX. Finished the first week of assignments for my DBMS course. 🤩

### R1D17 07/04/19
SQL @treehouse - Querying Relational Databases (Joins and Unions)
Working on my CPAsCode site to set up my professional portfolio and blog @wordpressdotcom

### R1D18 07/05/19
Starting a new webseries "Coding for Accountants" with Jahan Zahid.

The series will be broken up as follows:
Part 1: Setting up your coding environment, loading data from a CSV file
Part 2: Filtering and sorting data, function basics, adding new columns
Part 3: Plotting data using pie charts, bar charts, scatter plots, and more
Part 4: Pivot tables, create an aged debtors report, other data aggregation techniques
Part 5: Setting the scene for our machine learning problem and approach taken
Part 6: Implementing the machine learning algorithm to create a predictive model

-#Coding: Its Not Just for Programmers
https://www.accountingweb.co.uk/tech/tech-pulse/coding-for-accountants-its-not-just-for-programmers

-#Coding for Accountants Part One: An Introduction to Coding with AI
https://www.accountingweb.co.uk/tech/tech-pulse/coding-for-accountants-an-introduction-to-coding-and-ai

-#Coding for Accountants Part Two: Filtering and Sorting Data
https://www.accountingweb.co.uk/tech/tech-pulse/coding-for-accountants-part-two-filtering-and-sorting-data

-#Coding for Accountants Part Three: Plotting Data with Python
https://www.accountingweb.co.uk/tech/tech-pulse/coding-for-accountants-part-three-plotting-data-with-python

-#Coding for Accountants Part Four: Creating an Aged Debtors Report
https://www.accountingweb.co.uk/tech/tech-pulse/coding-for-accountants-creating-an-aged-debtors-report

-#Coding for Accountants Part Five: How to Build a Machine Learning Algorithm
https://www.accountingweb.co.uk/tech/tech-pulse/coding-for-accountants-how-to-build-a-machine-learning-algorithm

-#Coding for Accountants Part Six: Training a Machine Learning Algorithm

### R1D19 07/06/19

### R1D20 07/07/19

### R1D21 07/08/19

### R1D22 07/09/19

### R1D23 07/10/19

### R1D24 07/11/19

### R1D25 07/12/19

### R1D26 07/13/19

### R1D27 07/14/19

### R1D28 07/15/19

### R1D29 07/16/19

### R1D30 07/17/19

### R1D31 07/18/19

### R1D32 07/19/19

### R1D33 07/20/19

### R1D34 07/21/19

### R1D35 07/22/19

### R1D36 07/23/19

### R1D37 07/24/19

### R1D38 07/25/19

### R1D39 07/26/19

### R1D40 07/27/19

### R1D41 07/28/19

### R1D42 07/29/19

### R1D43 07/21/19

### R1D44 07/22/19

### R1D45 07/23/19

### R1D46 07/24/19

### R1D47 07/25/19

### R1D48 07/26/19

### R1D49 07/27/19

### R1D50 07/28/19

### R1D51 07/29/19

### R1D52 07/30/19

### R1D53 07/31/19

### R1D54 08/01/19
### R1D55 08/02/19
### R1D56 08/03/19
### R1D57 08/04/19
### R1D58 08/05/19
### R1D59 08/06/19
### R1D60 08/07/19
### R1D61 08/08/19
### R1D62 08/09/19
### R1D63 08/10/19
### R1D64 08/11/19
### R1D65 08/12/19
### R1D66 08/13/19
### R1D67 08/14/19
### R1D68 08/15/19
### R1D69 08/16/19
### R1D70 08/17/19
### R1D71 08/18/19
### R1D72 08/19/19
### R1D73 08/20/19
### R1D74 08/21/19
### R1D75 08/22/19
### R1D76 08/23/19
### R1D77 08/24/19
### R1D78 08/25/19
### R1D79 08/26/19
### R1D80 08/27/19
### R1D81 08/28/19
### R1D82 08/29/19
### R1D83 08/30/19
### R1D84 08/31/19
### R1D85 09/01/19
### R1D86 09/02/19
### R1D87 09/03/19
### R1D88 09/04/19
### R1D89 09/05/19
### R1D90 09/06/19
### R1D91 09/07/19
### R1D92 09/08/19
### R1D93 09/09/19
### R1D84 09/10/19
### R1D95 09/11/19
### R1D96 09/12/19
### R1D97 09/13/19
### R1D98 09/14/19
### R1D99 09/15/19
### R1D100 09/16/19


