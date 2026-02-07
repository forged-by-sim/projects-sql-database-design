🧱 Ages Table – Cross-Engine SQL Practice

Folder: ages-table-project
Focus: Creating and querying a basic SQL table using both MySQL and SQLite with interchangeable logic.

⸻

🧰 Tools & Environments

SQLite (via DB Browser)

MySQL/MariaDB (via shell or GUI)

VS Code for editing .sql and .txt

Python (sqlite3) – light testing for engine behavior

⸻

🔧 Steps Performed

Created the Ages table with two columns: name (TEXT/VARCHAR) and age (INTEGER)

Inserted a randomized list of name-age pairs

Queried the first alphabetical result using ORDER BY and LIMIT

Verified row counts and sanitized outputs

Captured results in GUI (output_firstrow.png) and tested compatibility

⸻

🧠 Core SQL Used

-- Create Table
CREATE TABLE Ages (
  name TEXT,
  age INTEGER
);

-- Insert Records
INSERT INTO Ages (name, age) VALUES ('Akam', 13);
INSERT INTO Ages (name, age) VALUES ('Aleesheh', 25);
...

-- Query First Alphabetical
SELECT name, age FROM Ages ORDER BY name LIMIT 1;


Optional challenge included computing an MD5 hash token (not available in all SQLite builds).

⸻

🔍 Troubleshooting Notes

Ensure case-sensitive table names are respected (Ages vs ages)

Confirm correct DB is selected in MySQL (USE demo_db;)

Use utf8mb4 to avoid encoding issues in MySQL

SQLite requires no DB selection — file-based logic only

⸻

💡 Reflection

This exercise emphasized reproducibility, syntax flexibility, and how to write portable .sql scripts. It mirrors small database tasks often needed for simulation scenarios like logging user sessions, creating test patient profiles, or storing runtime events for analytics.
