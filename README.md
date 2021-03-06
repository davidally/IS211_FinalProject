# POST.it

## TRY A LIVE VERSION OF THE APP!
## Hosted at: http://davidally.pythonanywhere.com/

## Possible Bugs
1) Login may require you to copy and paste your information to log in rather than type. This doesn't always happen but if it does, that is the fix. This will be worked on at a later date. 

Please open an issue if you encounter any bugs when using the app. 

## About POST.it

A full stack blog application where users can register and create/customize their own accounts. Once logged in 
they are able to make posts to the main page where others are also visible. Users can edit or delete their posts and account information.

## Running POST.it locally

Clone this repo then activate your virtual env in the directory.  
Next run:
```sh
#Install all required packages
pip install -r requirements.txt
```

Then simply run:
```sh
python run.py
```
Open localhost:5000 on your browser to view the web application.

The application will be empty upon opening, so you should Register an account then move on to create some posts to see it in action.

## How It Works

This is a blogging application written in Python using the Flask framework.  
Design Pattern: MVC 

The application is packaged in a folder which includes 3 modules for each part of the MVC
pattern. The `models.py` contains the classes that form the structure each user's data including their posts. The views are contained in `forms.py` using the FlaskForm module from the flask addon WTForms. The classes in this module are what build the forms you see on the front-end, albeit accessed through the Jinja templating. Finally, the controller connecting the two would be our `routes.py`. Several methods and decorators here do various things from tracking user sessions, redirects, authentication, image resizing, and more. The backbone of this application utilizes SQLAlchemy and Sqlite3 for the database as well as the package LoginManager which also is used for authentication.
