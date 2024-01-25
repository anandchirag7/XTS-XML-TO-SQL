# XTS-XML-To-SQL
Introducing XTS : An Automation Tool for Effortless Conversion of HANA Graphical Views to SQL Queries

Having worked with HANA for nearly eight years, I often found myself grappling with the challenge of converting
graphical views into SQL statements. As my company transitioned to Snowflake in recent months,
this curiosity led me to develop a Python-based automation tool named XTS.
This tool streamlines the conversion process, providing a range of functionalities to enhance efficiency and reduce errors during the migration process.

Key Features:

1. Conversion to a Do Begin Block:
Converts HANA graphical views into a 'do begin' block, with each node calculation translated into SQL.
Facilitates error reduction, faster debugging, and fewer deployments by allowing the same code to be tested in the HANA production environment.

2. Single SQL Query Conversion:
Transforms the entire view into a single SQL query, providing a concise representation of the logic.

3. Snowflake CTE View Conversion:
Converts HANA graphical views into Snowflake Common Table Expression (CTE) views.
Offers the option to replace sources with Snowflake tables or views for direct deployment to Snowflake.

4. Snowflake SQL View Conversion:
Similar to option 2, converts the view into a single select query view, ready for direct creation in Snowflake.


Results:

After converting over 100+ views, the tool has demonstrated an impressive accuracy range of 85-90%.
The time taken per view is significantly reduced to just 5 seconds, showcasing the efficiency gains achieved through automation.

How does it Work :
1. If copying the app folder to you IDE, run the login.py file to start the application and go through the application flow.
2. In Case you copy the executable folder, just double click on the XmlViewConverter.exe file to run the app.

v1.0
1. Fixed the incorrect calculations conversions
V2.0 :
1. Fixed bug for join condition calculations not reflecting in the converted sql
2. fixed bug for schema name not reflecting in the converted sql
v3.0
1. Added Conversion of HANA graphical views to Snowflake CTE or SQL views with source convert to Snowflake objects
2. Added new UI fro source conversion
3. enhancement to filter and calculation conversion

Still to be worked on :
1. Currency conversion
2. Geo data

I'm kind of new to python, so my way of coding might not be the best but i'm always up for improvement. So if you see anything that can be improved,
do let me know.

For any further addition to the tool or have an idea for collaboration which
we can work on

Contact :
Email : anandchirag7@gmail.com

Credits and libraries used :
1. PysimpleGui
2. Pandas
3. hdbcli
4. pathlib
5. json
6. fileinput
7. xlsxwriter
8. jinja2
