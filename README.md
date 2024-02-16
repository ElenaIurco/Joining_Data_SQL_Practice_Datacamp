# 🎉 Welcome to the SQL Joins & Subqueries Party! 🎊

Hey there SQL rockstar! 👩‍🎤👨‍🎤 Get ready to join the data extravaganza and spice it up with subqueries using these awesome notes from my DataCamp SQL course. 🚀

## SQL Joins 101 🕺💃

### What's the Buzz about Joins? 🤔
SQL Joins are like the coolest collab in the database world! They bring together tables to create powerful connections and unveil hidden insights in your data.

### Joining Basics 💻
- **INNER JOIN:** Think of it as the ultimate squad. It only includes rows with matching values in both tables. No one's left out! 🤝
  
  ```sql
  SELECT *
  FROM table1
  INNER JOIN table2 ON table1.column = table2.column;
  ```

- **LEFT JOIN (or LEFT OUTER JOIN):** It's like inviting everyone from the left table and matching buddies from the right. Some might come solo, though! 🕺💔
  
  ```sql
  SELECT *
  FROM table1
  LEFT JOIN table2 ON table1.column = table2.column;
  ```

- **RIGHT JOIN (or RIGHT OUTER JOIN):** The right table rules the dance floor, and the left table fills in the gaps. Who said you can't have favorites? 🎩💃
  
  ```sql
  SELECT *
  FROM table1
  RIGHT JOIN table2 ON table1.column = table2.column;
  ```

- **FULL JOIN (or FULL OUTER JOIN):** This is the wild card party! Everyone's invited, even if they don't have a match. Expect some NULLs crashing the dance! 🤹‍♀️🎉
  
  ```sql
  SELECT *
  FROM table1
  FULL JOIN table2 ON table1.column = table2.column;
  ```

### Subqueries Shake-Up 🔄

Subqueries are like secret dance moves that add flair to your SQL game! Let's see how to use them under different SQL clauses:

### Subquery under SELECT 🎵
- **Joining under SELECT:** Spice up your columns by selecting the joined tables' attributes. It's like mixing beats for the ultimate sound! 🎧📊
  
  ```sql
  SELECT table1.column1,
        (SELECT column2
         FROM table2
         WHERE condition) AS subquery_result
  FROM table1;
  ```

### Subquery under FROM 🎬
- **Joining under FROM:** Set the stage by joining tables right from the start. The show begins with a seamless connection! 🎬🔗
  
  ```sql
  SELECT *
  FROM table1
      (SELECT * FROM table2 WHERE condition) AS subquery_table;
  ```

### Subquery under WHERE 🕺💡
- **Joining under WHERE:** Filter the groove! Add conditions based on the joined tables for a customized dance floor. 🕺💃
  
  ```sql
  SELECT *
  FROM table1
  WHERE column1 IN (SELECT column2 FROM table2 WHERE condition);
  ```

### Takeaway 🎤
SQL Joins and Subqueries turn your data into a dancing and singing spectacle! Master these moves, and you'll be the SQL star of the show. Now go, join the data party, and let the insights groove in! 🚀💃

Feel free to fork, star, or contribute. Let's keep the SQL party going! 🌐✨

Happy querying! 🎉
```
