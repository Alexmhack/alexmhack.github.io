## Django Tictatoe Game

This game is gonna be from the pluralsight django tutorial.

We will be making a user authentication system in django.
We will use django_crispy forms tags to make real simple and easy forms for login page.

Users can also send game invitations to other users in the database, for simple usages wewill use the SQlite3 database that comes
preinstalled with django.

### Tictactoe Game
The tictactoe game will have the same functionality but with the help of forns user can enter his/her movoes.

With the help of python we will make simple game moves and handle the wining and losing users data

### Steps for Django Game

1. Create virtualenv for our django project using the terminal, if you don't have virtaulenv
	installed then install it using the pip command, to know why virtualenv is important visit [virtualenv importance](https://www.getfilecloud.com/blog/working-with-virtualenv-on-django-projects/)

	```markdown

	$ pip install virtualenv
	$ virtualenv env

	```

	here the virtualenv is the module which is invoked on our call and 'env' is the folder in which
	our virtual environment will be saved

2. Now the first thing after opening every terminal for our project is to activate our 
	virtualenv by entering this in the terminal

	```markdown

	$ env\Scripts\activate

	```

	You can clearly guess from this command, that we are calling the command 'activate' which is
	located inside the env\Scripts folder, you can peek into the folder and you will find it 
	there, one other similar command is 

	```markdown

	$ env\scripts\activate

	```
	
	This will also work

3. Once you have activated the env you can install the necessary packages among which, yeah you 
	guessed right, django is the one we need and work with most in our project

	```markdown

	$ pip install django

	```
	
	the pytz module installed with django is for the timezones for our django server

4. Now enough of the drama, start the django project

	```markdown

	$ django-admin.py startproject tictactoe

	```

	You can look at the tictactoe folder containing a file and a folder

	```markdown

	+ django_tictactoe_game
		+ tictactoe
		+ manage.py

	```

5. The first thing you should do and it is the most exciting for us beginners in django is to
	actually start the server and watch our project go live locally on our systems

	inside the folder where your manage.py file lies run this command in terminal, you should
	see something like this
	
	```markdown

	$ python manage.py runserver

	Performing system checks...

	System check identified no issues (0 silenced).

	You have 14 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, 	contenttypes, sessions.
	Run 'python manage.py migrate' to apply them.
	July 17, 2018 - 11:30:30
	Django version 2.0.7, using settings 'tictactoe.settings'
	Starting development server at http://127.0.0.1:8000/
	Quit the server with CTRL-BREAK.

	```
	
	**just ignore the warning for now, we will discuss those in next step.**
	
	Visit link http://127.0.0.1:8000/ in your browser and you can see the django welcome page.
