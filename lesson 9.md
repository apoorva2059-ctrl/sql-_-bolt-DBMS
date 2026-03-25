1.List all movies and their combined sales in millions of dollars
SELECT Title, (Domestic_sales + International_sales) / 1000000 AS Sales
FROM Movies
INNER JOIN Boxoffice
ON Movies.Id = Boxoffice.Movie_id;

2.List all movies and their ratings in percent
SELECT Title, Rating * 10 AS Rating_Percent
FROM Movies
INNER JOIN Boxoffice
ON Movies.Id = Boxoffice.Movie_id;

3.List all movies that were released on even number years
SELECT *
FROM Movies
WHERE Year % 2 = 0;
