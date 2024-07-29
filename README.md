# SQL-Interview-Questions

1) How do you switch to the imdb database?
------------------------------------------
        USE imdb;

2) How do you list all tables in the current database?
-------------------------------------------------------
       SHOW tables;

3) How do you display the structure of the movies table?
---------------------------------------------------------
       DESC movies;

4) How do you select all colo=umns from the movies table?
----------------------------------------------------------
       SELECT * FROM movies;

5) How do you select the name and year coulmns from the movies table ?
-------------------------------------------------------------------
       SELECT name, year FROM movies;

6) How do you select the rank score and name coulmns from the movies table ?
----------------------------------------------------------------------------
       SELECT rankscore,name
       FROM movies;

KeyWords
--------
       LIMIT
       -----
              Restricts the number of rows returned in the result set.

       OFFSET
       ------
              Specifies the number of rows to skip before starting to return rows.

7) How do you get the first 20 rows of name and rankscore from movie?
------------------------------------------------------------------------
       SELECT name, rankscore
       FROM movies
       LIMIT 20;

8) Why to use LIMIT and OFFSET?
----------------------------------------------------------
          LIMIT --> Efficient Resource Usage
          OFFSET --> Enables Pagination

9) How do you get 20 rows of name and rankscore starting from the 41st row in movies?
--------------------------------------------------------------------------------------
       SELECT name, rankscore
       FROM movies
       LIMIT 20
       OFFSET 40;

ORDER BY
---------
        The ORDER BY clause in SQL is used to sort the result set by one or more columns. By default, it sort in ascending order (ASC), but you can specify descending order (DESC) if needed.


10) How do you list the top 10 most recent movies by year showing name, rankscore, and year?
--------------------------------------------------------------------------------------------
        SELECT name, rankscore,year 
        FROM movies
        ORDER BY year DESC
        LIMIT 10;
        
