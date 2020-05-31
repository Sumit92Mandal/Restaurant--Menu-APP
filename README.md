# Restaurant--Menu-APP
 I have created Restaurant Menu app website using python ,flask and HTML. In which We can view respective hotel and their menu according to our choise, and also we can make changes in menus or in restaurant.

## Required :
1. Object-Oriented Python
2. SQL
3. HTML & CSS
4. git
5. vagrant
6. flask frameWork 
7. SQLAlchemy on an SQLite database

Before we perform any operations, we must first import the necessary **libraries**, connect to our restaurantMenu.db, 
and create a session to interface with the database:

### code  :
from sqlalchemy import create_engine 

from sqlalchemy.orm import sessionmaker 

from database_setup import Base, Restaurant, MenuItem

engine = create_engine('sqlite:///restaurantMenu.db') 

Base.metadata.bind=engine

DBSession = sessionmaker(bind = engine)

session = DBSession()

Then  perform **CRUD** (create ,Read, Update, Delete) operation on restaurantMenu.db <br>
**webserver.py** is the webservice code written in python that uses your restaurantMenu.db database to implement CRUD operation .
so, you can see the name of restaurant also can create ,delete or update the name of respective Restaurant.
## some screenshot of Restaurant name
<img src="images/restaurant.png " width=700 height =400 >

We have use **flask** frameWork  to create menu and code in **project1.py**.<br>
so that we can create new name in menu section.
also we can delete ,rename the corresponding restaurant menu items.<br>
Flask depends on the Jinja template engine and the Werkzeug WSGI toolkit. The documentation for these libraries 
can be found at: Jinja documentation.
The Flask code written in python with the help of HTML and css

## some screenshot of Menu
 <img src="images/menu.png " width=700 height =400 > 
 And, we can also edit /delete the menu of respective restaurant.
 
 ## Note :
  I have learnt this from Udacity full stack course.
