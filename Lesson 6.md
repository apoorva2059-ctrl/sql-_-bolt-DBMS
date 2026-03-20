Find the domestic and international sales for each movie ✓
SELECT Title,Domestic_sales, International_sales FROM Boxoffice INNER JOIN
Movies on Boxoffice.movie_id = Movies.id;

Show the sales numbers for each movie that did better internationally rather than domestically✓
SELECT Title,Domestic_sales, International_sales FROM Boxoffice INNER JOIN
Movies on Boxoffice.movie_id = Movies.id 
WHERE International_sales > Domestic_sales;


List all the movies by their ratings in descending order✓
SELECT Title,Rating FROM Boxoffice INNER JOIN
Movies on Boxoffice.movie_id = Movies.id 
order by Rating desc;
