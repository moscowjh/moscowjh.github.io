---
layout: post
title:  "Database Management is Tricky!"
---
I have done enough different things with data over the past year that I am finding it necessary to go back to review some basics. I recently started to review SQL since this is a skill that comes up in almost every real-life vacancy involving data science, analysis or engineering.

Working with an RDBMS (a relational database management system) by using SQL (structured query language) is relatively straightforward. It helps to have studied some database theory and relational algebra, but there are plenty of tutorials to teach basic commands and sample data on which to practice. In case any reader is interested in learning, Khan Academy has a pretty excellent [Intro to SQL sequence](https://www.khanacademy.org/computing/computer-programming/sql).

The [Udemy SQL course](https://www.udemy.com/the-complete-sql-bootcamp/) I am using for the review required me to set up a database server on my own computer as opposed to the common practice of offering a cloud-hosted environment to interact with in a browser window. Though conceptually easy, installing Postgres SQL on my Mac took a surprisingly long time because there are a number of ways to do it and I had to figure out which would work best for the exercises in the tutorial.  Within a couple hours, I did have Postgres running locally and was able to start the tutorials and assessments.

As often happens, I made my own life more complicated because I decided to download specific data as a Postgres database so that the exercises would be more engaging for me. I love baseball statistics and recalled that one of the best aggregations of historical baseball data is available as a SQL database! I estimated that downloading and getting it to run would be a 15 minute task.

That proved to be far from the case. First, it turned out that the SQL file of the baseball data works only for Microsoft SQL, so when I tried to import it into Postgres, the database schema was not created and Postgres would not import any data.  After a quick Google search, I found some scripts that are supposed to create the right schema and then import the data from CSV files. I tried that and, at first, they wouldn't work at all.

It turned out that if I launched the script using a command line editor, the permissions were messed up and wouldn't allow the import. So I found a different way to run the scripts and was able to quickly create the schema. But the data import still wouldn't work! Through trial and error, I discovered that I could get the data to import if I imported one file at a time. Since there are something like 26 files, it is possible to run through these one at a time. However, I want to make sure that I can then backup the database in way that allows me to reload it very easily. Total time burned was something like 3-4 hours and I still have not finished the task.

This reminded me of something that was very clear to me back in my web development days:
- database systems (including RDBMS) are very finicky and require precision to administer;
- the skillset required to manage databases is very different from what makes developers or data scientists successful;
- I am very comfortable using SQL to look up data and even to create basic reports, but much less at ease creating databases or modifying database structure.

Fortunately, this is an area where I'm pretty sure that I don't want or need to advance my skills much beyond where they are already.
