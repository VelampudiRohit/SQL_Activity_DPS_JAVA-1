# SQL_Activity_DPS_JAVA
SQL Activities for Genesis 2021

1. Create the table name: productions
* ```
CREATE TABLE productions (
    Productionid INT(5) PRIMARY KEY, 
    Productionname VARCHAR(30), 
    Address VARCHAR(40), 
    Startyear YEAR, 
    Ownername VARCHAR(20) 
    );
```
* ```
INSERT INTO productions VALUES 
(9091,"Arkamediaworks","Hyderabad",2001,"Shobu Yarlagadda"),
(8892,"Lyca Productions","Chennai",2014,"Subaskaran"),
(1010,"Hari Om Entertainment","Mumbai",2008,"Akshay Kumar"),
(1988,"Red Chillies Entertainment","Mumbai",2003,"Shah Ruck"),
(1899,"Viacom18 Studios","Mumbai",2008,"Ajit Andhare"),
(7882,"DVV Entertainments","Hyderabad",1993,"DVV Danayya"),
(6773,"Hombale Flims","Bangalore",1995,"Vijay"),
(7682,"Mythri Movie Makers","Hyderabad",2015,"Naveen Yerneni"),
(1854,"Junglee Pictures","Mumbai",2014,"Vineeth Jain"),
(2341,"CRM","Bangalore",2017,"Manohar")
,(1111,"STP","Chennai",2018,"Sree");
```

2. Create the table name: movie
* ```
CREATE TABLE movie (
    Movieid INT(5) PRIMARY KEY, 
    Moviename VARCHAR(30), 
    Heroname VARCHAR(30), 
    Heroine VARCHAR(30),
    Releaseddate DATE, 
    Language VARCHAR(15), 
    Length INT(2), 
    Movietype VARCHAR(25), 
    Productionid INT(5),
    FOREIGN KEY (Productionid) REFERENCES productions(Productionid)
    );
```
* ```
INSERT INTO movie VALUES 
(201,"Bahubali – The Beginning", "Prabhas", "Tamannah",20150710,"Telugu",21," Drama Fantasy", 9091),
(501,"2.0", "Rajnikanth", "Amy",20181129," Tamil", 20,"Scientific", 8892),
(577, "Aval", "Siddharth", "Andrea", 20171103, "Tamil", 14 ,"Horror", 1899),
(101, "Holiday", "Akshay Kumar" ,"Sonakshi" ,20140606, "Hindi" ,15 ,"Crime Thriller", 1010),
(151, "Zero", "Shah ruck" ,"Katrina Kaif", 20181221 ,"Hindi" ,16, "Scientific" ,1988),
(131, "Padmavaat", "Shahid Kapoor" ,"Deepika Padukone" ,20180125 ,"Hindi" ,21 ,"Drama Epic" ,1899),
(146, "Andhadhun", "Ayushmann", "Radika Apte", 20181005 ,"Hindi", 16 ,"Crime Thriller", 1899),
(231, "Bharath Ane nenu", "Mahesh Babu" ,"Kiara" ,20180420 ,"Telugu" ,15 ,"Thriller", 7882),
(244, "Gruham", "Siddharth" ,"Andrea" ,20181117 ,"Telugu" ,14 ,"Horror", 1899),
(337, "K G F chapter 1", "Yash" ,"Srinithi Shetty" ,20181221 ,"Kannada" ,21 ,"Action Thriller", 6773),
(224, "Rangasthalam", "Ram Charan", "Samatha" ,20180330, "Telugu", 17 ,"Drama Period", 7682),
(136, "Badhaai Ho", "Ayushmann", "Neena" ,20181018, "Hindi" ,14, "Drama Comedy", 1854),
(441, "The Villain", "Sudeep" ,"Amy" ,20181018, "Kannada", 16 ,"Drama", 2341),
(206, "Maryada Ramanna", "Sunil", "Saloni", 20100723, "Telugu" ,19 ,"Drama", 9091),
(211, "Khaidi No. 150", "chiranjeevi" ,"Kajal" ,20170111, "Telugu", 20 ,"Drama Thriller", 8892),
(188, "Rangoon", "Saif Ali Khan", "Kangana", 20170224 ,"Hindi" ,15 ,"Drama", 1899),
(189, "The House Next Door", "Siddharth", "Andrea", 20171110 ,"Hindi", 14 ,"Horror", 1899),
(267,"Anaganaga O Dheerudu", "Siddharth", "Shruthi", 20140114, "Telugu" ,16, "Fantasy", 9091);
```

## SQL Fundamentals Query
1. Display the name of movies, movie type is starts with Drama: 
2. Display the movies acted by actor Ayushmann:
3. Display the count of movies, having length above 18:
4. Display the movie having minimum length:
5. Display all the details of movie, the language that first name starts with ‘T’:
6. Display the movie name, hero name, heroine name whose having maximum length:
7. Display the movie name, hero name, heroine name the movie released after 15 march 2018:
8. Display the count of thriller movies:
9. Display the count of movies whose released before 15 march 2018:
10. Display the release date of the movie name ‘Zero’:
11.Display the actor name that acted with ‘Amy’:
12.Display the Count of maximum movies released in a month of October:
13.Display the movienames whose production id is same for different languages:

## SQL Advanced Query
1. Write the query to display productionid, production name with total number movies produced by each.
2. Write the query to display production name, owner name have produced more than 2 movies.
3. Write the query to display production name, owner name have produced maximum movies
4. Write the query to display the moviename, heroname and productionname acted in the producer name= ’Subaskaran’.
5. Write the query to display the moviename, heroname whose productionid ends with 82.
6. Write the query to display the productionname, ownername who has not produced the movie.
7. Write the query to display the productionname, ownername who has not produced the ‘hindi’ movie.
8. Write the query name to display the heroinename who acted in the different productions but not in same production id.
9. Write the query to display the heroname who acted in maximum languages.
10. Write the query to display the production name, owner name who has produced movie for more languages.
11. Write the query to display the productionname, producername who has not produced any movie.