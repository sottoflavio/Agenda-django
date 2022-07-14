# SCGHEDULE USING PYTHON + HTML
#### Video Demo:  https://youtu.be/v9hBX2UKFS0
#### Description:


This project is an experiment using PYTHON and HTML
To develop this project, I used the framework known as DJANGO
This framework made it possible to create a database system that will be hosted on a server
I created add, edit, remove records functions
In addition to security checks, so that a user cannot access the records just by having the URL, but having to go through a login.
Still about security, each user can only view their data in the agenda, not being able to see other users.

When the event is within 1 hour of its start, it appears in red, when the event has passed (one hour after its start) it is automatically hidden from the agenda.

The idea was to show the flexibility of the Django and Python framework for web development.
I chose not to create CSS styles and make the schedule as simple as possible, as the focus was initially on handling the data in the database.
For the database, I used SQLite because it is fast and has little data to handle.

the manage.py file is the application's main file, generated by the framework, which directs the operation through the main function.
db.sqlite3 file is our database, it can be easily migrated to another database in case of higher data flow.

inside the templates folder we have the HTML files that are our pages to be navigated.

Although I opted for the simple aspect of the page, they were made seeking the greatest possible reuse of code.

inside the core folder, is the core of our application, the files apps.py __init__.py, admin.py are files generated by the framework where I made the necessary adjustments for the application to work.
Inside the models file is the file that the framework uses to create the database and functions related to the data.

the views.py file generates the views for our HTML code and its functions according to the desired URL.

inside the agenda folder, in addition to the files generated by the framework, the most important thing I coded was urls.py that tells us which of the functions the views file will use according to the desired url.