# How to get started
1. Install Pycharm Professional (1 month trial, but free if you sign up as student) Or VScode and Install node.js
2. When you first open Pycharm, it'll ask "Open Project/ Open Folder" choose the folder where you downloaded the "Project1"
3. If Pycharm asks to install any packages (like javascript) click yes and wait for it to finish installing 

4. Whenever you start any project, you want to enable a virtual environnment, you do that by typing
"virtualenv venv" into the Pycharm terminal (if  it doesn't work do "pip install virtualenv" first)

4b. To activate virtual environment on windows type "venv\Scripts\activate" for Mac I think it's  "source venv/bin/activate" or "venv/bin/activate"
-- if you get this error: "cannot be loaded because running scripts is disabled on this system."  Go to desktop search bar and run Windows powershell as Administrator and paste "set-executionpolicy remotesigned" into the command line, then you can activate

5. Then install all the packages needed type "pip install -r requirements.txt" into the command console

6. If it asks you to migrate anything in the console, these are the commands.
"python manage.py migrate" or
 <-- if it you get this error: "no such table: users_user" Run
"python manage.py makemigrations" + "python manage.py migrate --run-syncdb"

7. Then you run the server, aka to enable Back end.
"python manage.py runserver"

8. Then enable Front end by entering in a second terminal
"npm install" and "npm run build" + "npm start"

9. To get started you create a superuser if you want to make an admin account
"python manage.py createsuperuser"

