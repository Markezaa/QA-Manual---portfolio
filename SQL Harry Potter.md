

1\. **Print the first name, last name, and patronus of all characters who have a known patronus.**  
	SELECT fname, lname, patronus  
FROM characters  
WHERE NOT patronus \= 'Unknown' AND patronus IS NOT NULL;

2\. **Print the last names of characters whose last name ends with the letter 'e'.**  
SELECT \*  
FROM characters  
WHERE lname LIKE ("%e");

3\. **Calculate the total age of all characters and print it on the screen.**  
	SELECT sum(age) as “Total age”  
FROM characters;

4\. **Write names, last names and years of the characters in descending order of their years.**  
	SELECT fname, lname,age  
FROM characters  
ORDER BY age DESC;

5\. **Write names and years of the characters whose years are in between 50 and 100 years.**  
	SELECT fname, age  
FROM characters  
WHERE age BETWEEN 50 AND 100;

6\. **Print the ages of all characters without including duplicate ages.**  
	SELECT DISTINCT age  
FROM characters;

7\. **Print all information about characters whose faculty is Gryffindor and whose age is over 30\.**  
	SELECT \*  
FROM characters  
WHERE faculty \="Gryffindor"  
AND age\>30;

8**. Print the names of the first three faculties from the table without duplicates.**  
	SELECT  DISTINCT faculty  
FROM characters   
LIMIT 3;

9 . **Print the names of characters whose name starts with 'N' and has 5 letters, or whose name begins with 'L'.**  
SELECT fname  
FROM characters  
WHERE fname LIKE ("N\_\_\_\_" OR fname LIKE 'L%');  
	  
10\. **Calculate the average years of all characters.**  
	SELECT avg(age)  
FROM characters;

11\. **Delete character with** **ID \= 11\.**  
	DELETE FROM characters  
WHERE char\_id=11;

12\. **Print the last names of the characters that contain the letter “a”**.  
	SELECT lname   
FROM characters  
WHERE lname LIKE '%a%';

13\. **Use an alias to temporarily rename the column `fname` as 'Half-Blood Prince’**.  
	SELECT fname AS  Half\_Blood\_Prince  
FROM characters;

14**. Print the ID and names of all known patronuses in alphabetical order.**  
	SELECT char\_id,patronus  
FROM characters   
WHERE NOT patronus \=” Unknown” AND patronus IS NOT NULL  
ORDER BY patronus ASC;

15\. **Using the IN operator, print the first and last names of characters whose last name is Crabbe, Granger, or Diggory**  
	  
	SELECT fname,lname  
FROM characters  
WHERE lname IN ('Crabbe', 'Granger',' Diggory');

16\. **Print the minimum age of the characters.**  
	SELECT min(age)  
FROM characters;

17**. Use the UNION operator** **to print names from the characters table and book titles from the library table.**  
	SELECT fname FROM characters  
UNION  
SELECT book\_name FROM library;

18\. **Use the HAVING operator, calculate the number of characters per faculty, keeping only those faculties where the number of students is greater than 1**  
	SELECT faculty, COUNT(\*) AS broj\_studenata  
FROM characters  
GROUP BY faculty  
HAVING COUNT(\*)\>1;

19\. **Print the first name, last name of characters, and the title of the book they belong to..**  
SELECT c.char\_id,fname,lname,book\_name  
FROM characters c  
JOIN library l ON c.char\_id \= l.char\_id;

20\. **Print the first name and last name of characters and the title of the book, regardless of whether they have a book or not.**  
	SELECT c.char\_id,fname,lname,book\_name  
FROM characters c  
LEFT JOIN library l ON c.char\_id \= l.char\_id;

21\. **Print the book title and the name of the patronus, regardless of whether the information about the book owner is in the table or not.**

	SELECT c.char\_id,fname,lname,book\_name  
FROM characters c  
LEFT JOIN library l ON c.char\_id \= l.char\_id;

22\. **Print the first name, last name, and age of characters and the title of the book they belong to, provided that all book owners are older than 15 years.**

	SELECT c.char\_id,fname,lname, age,book\_name  
FROM characters c  
JOIN library l ON c.char\_id=l.char\_id  
WHERE age\>15;

23\. **Print the character's name, book title, release date, and end date, provided that the character is younger than 15 years old and their patronus is unknown.**

	SELECT c.char\_id,fname,lname, age,patronus,book\_name,start\_date,end\_date  
FROM characters c  
JOIN library l ON c.char\_id=l.char\_id  
WHERE age\<15  
AND patronus IS NULL;

24\. **Use a nested query to count the number of books whose `end_date` is later than Hermione's end\_date.**

SELECT COUNT(\*)   
FROM library  
WHERE end\_date \>(  
		SELECT end\_date FROM characters JOIN library ON characters.book\_id=library.book\_id WHERE characters.fname=”Hermione”);  
    		

25\. **Using a nested query, print the names of all patronuses whose owners are older than the character whose patronus is 'Unknown'.**

SELECT patronus  
FROM characters  
WHERE age \>(  
	SELECT age  
FROM characters  
    	WHERE patronus='Unknown');

	

