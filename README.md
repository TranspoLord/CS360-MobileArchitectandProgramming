# CS360-MobileArchitectandProgramming

# Summary of the requirements and goals of the app
The goal of this application is to track a simple database full of products and items for
an inventory. The user can add, edit, and delete items in the database, as well as searching
and browsing through the database.

# The screens needed for the app?
At least six screens were needed for the application. A login screen, main menu, browse, search, 
product add, and a product informatin screen. I believe my designs were successful with users
in mind because it got straight to the point. No unneeded features were added, no unneeded flaires
or other themes clashing with each other.

# How did you approach the process of coding my app
The coding of the app was strategic. I ended up completely restarting the project to help with this,
as my mind would've been too jumpy to actually get anything done. Plus, it helped a lot with debugging
and fixing errors. I started with the login portion where a database was created, specifically for 
logins and logins only. Knowing that the application would need a database for products as well, 
a database helper and seperate services for the databases were created. Once login was done, the
main menu code was created to allow going to and from different screens. In the browse and search
screen, code was added to pull the R, in CRUD, from the product service, to build the list with
buttons for each product in the database. Once the product button was selected, an intent was passed
to the product screen, giving the id of the product which would allow the activity to pull up
the correct product from the database. Once all the features were built, debuging along the way, 
final touches were added. 

# How did you test your code
A debug menu was added in with a link to the main menu. This menu was added with options to control
the databases as it was annoying and really time consuming to add products and/or drop the databases.
The menu allows the tester to populate the product database with a short list of products, delete
the product database, and delete the login database, among other things. The process was important
as it did help a LOT with time management, as well as revealing certain things in the application that
needed to be fixed. 
This menu was left in to help with the review of the application. If it was an actual release, the menu 
would be removed. The code would be left in as it would be needed for further updates and development.

# Where did you have to innovate to overcome a challenge?
One innovation was the SQLite database. I've always had a hard time with databases as all the syntax
sometimes confuse me. The problem was being able to contact the database without having to add the code
to each activity. Looking back at other projects from other classes, and an idea from a friend, the
database service was thought of and created. The services create and handle the databases in a CRUD like
format. A database helper provided a middle man that allowed each activity to talk to the services. 

# What specific component you were particularly successful in?
Aside from creating the database, which I am proud of, the browse and search screens are, also, great examples.
The screens needed to create a button for each product in the list, and create them dynamically, as to
not take up too many resoruces. Android itself actually does take care of the dynamic part, as each
button is added once the user scrolls far enough. The main issue was creating the button, adding it to the 
scroll layout, and then being able to pass the correct product, through intent, to the product screen. 
After researching it for a short while, I was able to figure out how to pass the correct product. I 
simply got the product ID, and passed it, where the product screen would get the product details by
searching the ID. This works because each ID is unique and another one cannot be created. 
