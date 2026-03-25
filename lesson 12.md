Find the number of movies each director has directed
SELECT Director, COUNT(Title) AS Amount_of_Movies FROM Movies GROUP BY Director;

Find the total domestic and international sales that can be attributed to each director
SELECT Director, SUM(Domestic_sales + International_Sales) AS Total_Sales
FROM Movies INNER JOIN Boxoffice ON Movies.Id = Boxoffice.Movie_Id GROUP BY Director;
