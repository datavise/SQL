# MIN & MAX

`SELECT substr(release_date, 0, 5) AS year, title,`&#x20;

`MAX(vote_average) as top_votes`&#x20;

`FROM movies`&#x20;

`GROUP BY year`&#x20;

`ORDER BY year DESC`



![](../.gitbook/assets/max.png)

