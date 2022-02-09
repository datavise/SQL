# GROUP BY

We can also add a GROUP BY statement to count the number of titles in each language, with a budget greater than 1000000:

![](../../.gitbook/assets/count\_group.jpg)

`SELECT original_language,`&#x20;

`substr(release_date, 0, 5) AS year,`&#x20;

`COUNT(title) as titles`&#x20;

`FROM movies`&#x20;

`WHERE budget > 1000000`&#x20;

`GROUP BY original_language, year`&#x20;

`ORDER BY year DESC`



![](../../.gitbook/assets/group\_two)
