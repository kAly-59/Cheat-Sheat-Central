#EXO SQL

## EXO 1:
1- Find the title of each film
``SELECT title FROM movies;``
2- Find the director of each film
``SELECT director FROM movies;``
3- Find the title and director of each film
``SELECT title, director FROM movies;``
4- Find the title and year of each film
``SELECT title, year FROM movies;``
5- Find all the information about each film
``SELECT * FROM movies;``

## EXO 2
1- Find the movie with a row id of 6
``SELECT * FROM movies WHERE id = 6;``
2- Find the movies released in the years between 2000 and 2010
``SELECT * FROM movies WHERE year BETWEEN 2000 AND 2010;``
3- Find the movies not released in the years between 2000 and 2010
``SELECT * FROM movies WHERE year NOT BETWEEN 2000 AND 2010;``
4- Find the first 5 Pixar movies and their release year
``SELECT * FROM movies WHERE year LIMIT 5;``

## EXO 3
1- Find all the Toy Story movies
``SELECT title FROM movies WHERE title LIKE "Toy Story%";``
2- Find all the movies directed by John Lasseter
``SELECT title FROM movies WHERE director = "John Lasseter";``
3- Find all the movies (and director) not directed by John Lasseter
``SELECT title FROM movies WHERE director != "John Lasseter";``
4- Find all the WALL-* movies
``SELECT title FROM movies WHERE title LIKE "WALL-%"``

## EXO 4:
1- List all directors of Pixar movies (alphabetically), without duplicates.
``SELECT DISTINCT Director FROM movies ORDER BY Director;``
2- List the last four Pixar movies released (ordered from most recent to least)
``SELECT title, year FROM movies ORDER BY year DESC LIMIT 4;``
3- List the first five Pixar movies sorted alphabetically
``SELECT title, year FROM movies ORDER BY title ASC LIMIT 5``
4- List the next five Pixar movies sorted alphabetically
``SELECT title, year FROM movies ORDER BY title LIMIT 5 OFFSET 5;``
