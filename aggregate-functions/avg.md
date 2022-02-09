# AVG

SELECT substr(release\_date, 0, 5) AS year,&#x20;

ROUND(AVG(budget), 2) as average\_budget&#x20;

FROM movies&#x20;

GROUP BY year&#x20;

ORDER BY year DESC



![](../.gitbook/assets/image.png)
