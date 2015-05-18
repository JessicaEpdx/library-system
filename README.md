#LIBRARYhelper

###By Jessica Engel & Erin Collins

LIBRARYhelper is a library system for administrators to keep track of library patrons, books, and copies. 

####Setup

Gemfile included bundle before use:

    $ gem install bundler
    $ bundle

Building the database in postreSQL:

    $ psql
    username=# CREATE DATABASE library;
    username=# \c library;
    library=# CREATE TABLE copies (id serial PRIMARY KEY, book_id integer, number_of_copies integer);
    library=# CREATE TABLE books (id serial PRIMARY KEY, title varchar, author varchar);
    library=# CREATE TABLE patrons (id serial PRIMARY KEY, name varchar);
    library=# CREATE DATABASE library_test WITH TEMPLATE library;

####Github Access

For any debugging questions contact JessicaEpdx@gmail.com

####License

MIT License. Copyright 2009-2015 Jessica Engel
