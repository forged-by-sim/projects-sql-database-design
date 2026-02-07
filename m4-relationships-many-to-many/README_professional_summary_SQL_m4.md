🔗 M4 – Many-to-Many Relationships & JSON Export

Folder: m4-relationships-many-to-many
Focus: Designing normalized schemas with many-to-many relationships and exporting relational data into structured JSON format.

⸻

🎯 Overview

This module introduced how to structure complex relationships using a junction table, write multi-table SQL queries, and export the result to JSON — a critical bridge between relational logic and modern web/backend data formats. The project emphasized both schema design and cross-format data interoperability.

⸻

🛠️ Core Skills Practiced

Implementing many-to-many relationships using junction tables

Writing JOIN queries across User, Course, and Member tables

Using foreign keys to maintain referential integrity

Exporting SQL result sets to JSON format

Visualizing schema and exports with screenshots and GUIs

⸻

📁 Key Subfolder: schema-json-exports-project

This folder contains the full project pipeline from schema setup to data export:

File	                                        Purpose
user-course-schema.sql  	                Defines User, Course, and Member tables with inserts
user-course-roster.json	                        Final exported JSON result from the SQL JOIN query
schema-setup.png	                        Screenshot of ERD-style table structure with keys
query-output.png	                        Screenshot of final JOIN query result
json-export-preview.png	                        Screenshot of phpMyAdmin JSON export interface
json-prettyprint.png	                        Formatted JSON output for human readability
README_m4_schema_json_exports_project.md	Dedicated README documenting the export workflow

⸻

🖼️ Instruction Reference

These instructional files are retained for transparency and traceability:

File	                                                Purpose
json-instructions-1.png → json-instructions-4.png	Assignment and UI steps (original references)
stepbystep-json-export-guide.txt	                Full narrative walkthrough of schema → query → JSON
json-export-assignment-notes.txt	                Summarized breakdown of the export assignment

⸻

💡 Reflection

This module mirrored real-world use cases I often see in simulation backend systems — such as exporting session logs, user profiles, or role-course pairings. The ability to move between SQL JOINs and readable JSON is a powerful, transferable skill, especially when building tools that sync structured simulation data with front-end visualizations or XR pipelines.