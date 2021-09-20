# Backend - Database Basics - Show Me

You are planning to build an app where users can add poems anonymously. You want to have _some_ data regarding the poem, but nothing that can be used to identify the user. Before even starting, try to think about the data you will be handling. You (as an administrator) are allowed to edit the poems.

You could take some inspiration from here; https://www.poetryfoundation.org/poems/152825/

- What data to save?
save collection of poems

- Which types of fields would you have? Do you need dates?
title, author, created date, poem, published date

- Estimate how much data will you allow to be saved 

- Describe the data in whatever way you find best
- Show how you would create the table(s) for your data


CREATE DATABASE poems;

USE poems;

CREATE TABLE poem(
    title TEXT(100) NOT NULL,
    content TEXT(1000) NOT NULL,
    author TEXT(100),
    created DATETIME NOT NULL,
    published BOOLEAN NOT NULL
);