Commands
Show all the data in the owners table.
SELECT * FROM owners;

Show the names of all owners.
SELECT name FROM owners;

Show the ages of all of the owners in ascending order.
SELECT age FROM owners
ORDER BY name ASC;

Show the name of an owner whose name is Donald.
SELECT name FROM owners
WHERE name = 'Donald';

Show the age of all owners who are older than 30.
SELECT * FROM owners
WHERE age > 30;

Show the name of all owners whose name starts with an E.
SELECT * FROM owners
WHERE name LIKE 'E%';

Change Jane's age to 30.
UPDATE owners SET age=30 WHERE name ILIKE 'jane';

Change Jane's name to Janet.

UPDATE owners SET name='Janet' WHERE name ILIKE 'jane';

Delete the owner named Janet.

DELETE from owners WHERE name = 'Janet';

Show the names of the first three owners in your owners table.

SELECT name FROM owners LIMIT 3;