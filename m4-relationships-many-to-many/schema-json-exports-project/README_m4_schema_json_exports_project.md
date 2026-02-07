🧩 M4 – SQL Schema Join & JSON Export

Folder: schema-json-exports-project
Focus: Constructing a normalized schema with many-to-many relationships and exporting the JOINed output as a JSON file.

⸻

🎯 Overview

This project models a real-world user-course-role structure using SQL. I implemented foreign keys and junction tables to represent a many-to-many relationship, queried the output using multi-table JOINs, and exported the results to JSON using phpMyAdmin. The exported data was then formatted for clarity and downstream integration.

⸻

🛠️ Key Components
File	Purpose
user-course-schema.sql	Defines the schema and inserts sample data
user-course-roster.json	Final exported JOIN output in JSON format
schema-setup.png	Screenshot of table structure with foreign keys
query-output.png	Output of the SQL JOIN query
json-export-preview.png	phpMyAdmin JSON export interface
json-prettyprint.png	Cleaned, indented JSON file

⸻

🧠 Core SQL Logic

SELECT User.name, Course.title, Member.role
FROM User
JOIN Member ON User.id = Member.user_id
JOIN Course ON Member.course_id = Course.id;


This query flattens the relationships into a readable roster linking users, courses, and roles.

⸻

📤 JSON Export (Preview)

[
  {
    "name": "Akam",
    "title": "Python for Everybody",
    "role": 1
  },
  {
    "name": "Aleesheh",
    "title": "Web Development",
    "role": 0
  }
]


The result is suitable for web frontends, API responses, or simulation state syncs.

⸻

💡 Reflection

This was my first end-to-end workflow connecting relational schema logic to cross-platform data export. In the field of simulation tech, this is directly applicable — especially when storing user-event logs, converting training data to JSON, or feeding XR dashboards with structured backend data.