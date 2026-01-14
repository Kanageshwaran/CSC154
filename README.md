# CSC154
Computer System Attacks and Countermeasures

SQL Injection Attack and Defense Lab Overview

This lab focused on understanding and demonstrating SQL injection vulnerabilities in a deliberately insecure web application, followed by implementing secure coding techniques to prevent such attacks. The project analyzed how unsafe SQL query construction using user-supplied input can lead to unauthorized data access and data manipulation, and how proper defenses eliminate these risks.

Developed as part of coursework at California State University, Sacramento using the SEED Labs SQL Injection Attack Lab environment.

Project Objectives

-Understand how SQL injection vulnerabilities arise in web applications
-Exploit SQL injection in SELECT statements to bypass authentication and access protected data
-Exploit SQL injection in UPDATE statements to demonstrate unauthorized data modification
-Analyze why certain injection techniques fail due to built-in countermeasures
-Implement and verify defenses using prepared statements and parameter binding

Design & Implementation

The lab environment used a vulnerable PHP and MySQL web application in which user inputs were originally concatenated directly into SQL statements. The project involved identifying these insecure query patterns and replacing them with secure query mechanisms.

Attack Demonstrations

-SELECT statement injection to gain unauthorized access to sensitive user data
-UPDATE statement injection to modify database records without proper authorization

Defense Implementation (Prepared Statements)

The vulnerable SQL queries were rewritten using prepared statements with bound parameters. User inputs such as usernames and password hashes were passed as parameters instead of being embedded in SQL strings, preventing attacker-controlled input from being interpreted as executable SQL code. After applying these changes, SQL injection attempts failed while normal application functionality was preserved.

Technologies Used

-Linux (SEED Labs virtual environment)
-PHP (mysqli)
-MySQL / SQL
-Web application backend and frontend interaction
-Prepared statements and secure query handling

Learning Outcomes

This lab strengthened my understanding of how SQL injection compromises confidentiality and integrity in web applications, how insecure backend code enables these attacks, and why prepared statements are a fundamental defense. It also improved my ability to analyze vulnerable code, implement security fixes, and validate countermeasures through testing.
