CalendarSite is a web app developed using FullCalendar jquery plugin and asp.net.
I have used asp.net 3.5.

You dont need to change much, just make changes to the code in EventDAO class in App\_Code folder.

For storing events, i have used sql server express database. In that i have created a table named "event"

Here is the table format:
event(event\_id int, title varchar(100), description varchar(200),event\_start datetime, event\_end datetime)
event\_id is the primary key

So all you have to do to get this app working is, to make changes in EventDAO class. Basically just change the connection string and the names of the columns which you have used in your database.
The names of column used in my EventDAO class are as per the table 'event' shown above.

Plus see the comments in the class, if you have doubts.