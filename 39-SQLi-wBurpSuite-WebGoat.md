##  SQLi with Burp Suite, WebGoat

#### Readings <br/>
[Understanding SQL Injection, Identification and Prevention](https://www.varonis.com/blog/sql-injection-identification-and-prevention-part-1/)

---

SQL injection is a code injection technique that might allow an attacker to execute malicious SQL statements that control a web application's database server.

---

An example of how a hacker could use SQL injection to gain unauthorized access: If a web application's page uses a URL parameter to retrieve data from a database, the hacker could modify the URL parameter to include an SQL fragment that will be run by the database. An example of this is changing a legitimate URL from http://example.com/item?id=1 to http://example.com/item?id=1;DROP TABLE users;. If the application is vulnerable to SQL injection, this could lead to the deletion of the "users" table.

---

To prevent SQL injection attacks on a web server: <br/>

- Use prepared statements and parameterized queries which ensure that an attacker cannot change the intent of a query, even if SQL commands are inserted into the input.<br/>

- Employ stored procedures to use predefined SQL, which does not allow the attacker's SQL to be executed.<br/>

- Validate and sanitize all user inputs to prevent malicious data from affecting the logic of the query.<br/>

- Use web application firewalls to help identify and block SQL injection attempts.<br/>

- Keep the database systems, software libraries, and dependencies updated to mitigate known vulnerabilities.