📊 M2 – Select Queries & Cross-Engine Compatibility

Folder: m2-select-and-filtering
Focus: Writing basic SQL queries, understanding result filtering, and translating syntax between SQLite and MySQL.

⸻

🎯 Overview

This module introduced foundational SQL operations using a custom Ages table with randomized data. The primary goal was to build the table, insert values, and retrieve the first alphabetically sorted entry using both SQLite and MySQL engines.

⸻

🛠️ Core Skills Practiced

Writing CREATE TABLE, INSERT, and SELECT statements

Filtering results using ORDER BY, DESC, and LIMIT

Identifying syntax differences across SQL engines

Running scripts via GUI clients and command line

Using .sqlite files and .sql scripts in real-world scenarios

⸻

📁 Key Folder: ages-table-project

Contains scripts and assets for both engines:

ages-table-sqlite.sql → SQLite version

ages-table-mysql.sql → MySQL-compatible version

ages.sqlite → SQLite database file

output_firstrow.png → Screenshot of query result

ages_prompt.png → Visual of assignment/task prompt

stepbystep-ages-table-guide.txt → Walkthrough of table design

⸻

🧪 SQL Query Example
SELECT name, age FROM Ages ORDER BY name LIMIT 1;


This returns the first alphabetical entry and was run in both engines to validate query translation and consistency.

⸻

🔄 Compatibility Insights

This module helped solidify cross-platform awareness:

SQLite allows inline execution via DB Browser or CLI

MySQL/MariaDB requires creating and switching to a database (USE demo_db;)

Engine-specific quirks (e.g. case sensitivity, MD5 availability) were tracked and noted

⸻

💡 Reflection

This was my first end-to-end SQL workflow across two engines. While the logic was simple, it clarified the differences between database systems and how structured queries behave. As a simulation technologist, I can see how this logic maps to small-scale training records, user settings, or even prototype backends for XR tools.