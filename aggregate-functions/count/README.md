# COUNT

SQL has several aggregate functions, including COUNT, SUM, MIN, MAX, and AVG. Aggregate functions allow you to summarize a column by grouping or 'rolling up' the data.

`SELECT COUNT(title) as titles`&#x20;

`FROM movies`



![](../../.gitbook/assets/count.jpg)

We can also combine this with a WHERE statement to count the titles which have budgets greater than a million dollars:

![](../../.gitbook/assets/group.png)

