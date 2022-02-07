# Databases

A broad definition for a database is 'a computerized container for organized data'. This definition includes spreadsheets or plain text files such as XML or CSV.



Usually, however, when talking about a database, people usually mean relational database management systems or RDBMS.



**Relational Databases**

A database contains one or more tables, which should be familiar if you've ever created a sheet in a spreadsheet like Excel or Google Sheets. Each table has a row for each record and rows, in turn, are split into fields, as shown in the Movies table below:

**Movies Table**

| MOVIE\_ID | TITLE     | BUDGET   |
| --------- | --------- | -------- |
| 862       | Toy Story | 30000000 |
| 8844      | Jumanji   | 65000000 |
|           |           |          |

Each row contains a movie record, which has fields for its id, title, and budget. Each MOVIE\_ID is unique to a movie. No two movies have the same MOVIE\_ID.



The Movies table could have a related **Ratings Table**:

| USER\_ID | MOVIE\_ID | RATING |
| -------- | --------- | ------ |
| 1        | 862       | 3      |
| 4        | 862       | 4      |
| 4        | 8844      | 3      |

A relationship exists between the two tables because the MOVIEID in the Ratings table refers to the MOVIE\_ID of the movie in the Movies table.

Note that in the Ratings table, MOVIE\_IDs are not unique. Many different users can have a rating for one movie. The Movies table contains a single row for each movie - and the related Ratings table contains a record for each rating.



**Why are tables split like this in relational databases?**

This method of splitting tables via a relationship is called **normalization** and helps to keep from repeating the data in the database. Each movie only needs to have its title and budget information stored **once**, not every time there's a new rating.

This approach of structuring the data so it isn't duplicated also helps with maintaining the database. If we needed to amend the movie's title, we would only need to update it in one place.

