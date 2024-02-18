# 💽 Local: Development
   
 * `pip install django` 
 * `django-admin startproject romanianmovies`
 * `cd romanianmovies`
 * `manage.py startapp movie`
 * `python manage.py startapp accounts`
 * `python manage.py startapp news`
 * `python manage.py makemigrations`
 * `python manage.py migrate`
 * `python manage.py createsuperuser`
 * `python manage.py runserver`
  
### https://127.0.0.1:8000/admin and login with credentials
 or<br>
docker-compose up<br>
http://localhost:8000/

##  Production https://www.pythonanywhere.com/
I used PythonAnywhere to host Python-based web applications directly from the platform. It supports web frameworks such as Django, Flask, and web2py, among others.

1. git clone https://github.com/mariabb/romanianmovies.git  (clone the Repository from git hub, this is the name in my case)
2. create a virtual environment , “venv” is the name :
`mkvirtualenv venv`
3. `cd romanianmovies `
4. To install the packages listed in a requirements.txt file, run the command: 
`pip install -r requirements`
5.open the settings file in Web section and modify the path, then:
* `DEBUG = True`
* `ALLOWED_HOSTS = [‘https://mariab.pythonanywhere.com/’] `
6. To  upload images, additional settings are required; see the instruction s here: https://www.pythonanywhere.com/
In WEB section, I added:
* url:`/static `, Directory: `/home/mariab/romanianmovies/static `
* url:`/media/ ` , Directory: `/home/mariab/romanianmovies/media `
* https://mariab.pythonanywhere.com/
  
