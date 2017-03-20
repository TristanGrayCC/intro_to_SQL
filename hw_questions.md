# SQL Homework Questions

Use the supplied data as the source of data to answer the questions.  Copy the SQL command you have used to get the answer, and paste it below the question, along with the result they gave.

## Questions

1. Return ALL the data in the 'movies' table.
    SELECT * FROM movies;
2. Return ONLY the name column from the 'people' table
    SELECT name FROM people;
3. Oops! Someone at CodeClan spelled John's name wrong! Change it to reflect the proper spelling (change 'jhn Harper' to 'John Harper').
    UPDATE people SET name = 'John Harper' WHERE id = 14;
4. Return ONLY your name from the 'people' table.
    SELECT name FROM people WHERE id = 8;
5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
    DELETE FROM movies WHERE id = 9;
6. Create a new entry in the 'people' table with the name of one of the other instructors (Tony, Kat, etc).
    INSERT INTO people (name) VALUES ('Tony Portugese');
7. Zsolt, has decided to hijack our movie evening, Boo! Remove him from the table of people.
    DELETE FROM people WHERE id = 9;
8. Somehow the list of people includes two people named 'instructor'. Change these entries to the proper names ('Darren Breen', 'Sandy McMillan')
    UPDATE people SET name = 'Darren Breen' WHERE id = 10;
    UPDATE people SET name = 'Sandy McMillan' WHERE id = 11;
9. The cinema has just heard that they will be holding an exclusive midnight showing of 'Guardians of the Galaxy 2'!! Create a new entry in the 'movies' table to reflect this.
    INSERT INTO movies (title, year, show_time) VALUES ('Guardians of the Galaxy 2', 2017, '00:00');
10. The cinema would also like to make the Guardian movies a back to back feature. Update the 'Guardians of the Galaxy' show time from 12:10 to 21:30
    UPDATE movies SET show_time = '21:30' WHERE id = 11;

## Extension

1. Research how to delete multiple entries from your table in a single command.
    DELETE FROM movies WHERE year BETWEEN 2008 AND 2011;
    DELETE FROM movies WHERE id IN (12,7);
