


Django is an open-source python web framework used for rapid development, pragmatic, maintainable, clean design, and secures websites. A web application framework is a toolkit of all components need for application development. The main goal of the Django framework is to allow developers to focus on components of the application that are new instead of spending time on already developed components. Django is fully featured than many other frameworks on the market. It takes care of a lot of hassle involved in the web development; enables users to focus on developing components needed for their application.

step1- Create an Project using Command:
 $ django-admin startproject (projectname)

  They create an directory name as project name. In projectname folder there are few files are created that is 
  . __init_.py
  . setting.py
  . urls.py
  . wsgi.py
  . manage.py

  From all for these files two files are main and mostly used in this project that is 
  . urls.py
  . setting.py
  . manage.py

Step2:-  Run the server . To run the server we have to stay in the same directory and run the command:

$ py manage.py runserver

After this execution, it show's a utls and that url shows  the django successfully working web page.


Step3:- Create an app for our Project. In django project app is used to provide the functionality to our webpages. how link works 

$ py manage.py startapp appname

After Creating an app folder first thing is to do is add app name in the project setting.py folder under INSTALLED APPS section.

In django,build in sqlite database that store all data in the admin panel.

I have also shared the screenshots for the same.



 


Django by default provides an authentication system configuration. User objects are the core of the authentication system.today we will implement Django’s authentication system.

django based login,logout and register system [django docs on auth system](https://docs.djangoproject.com/en/2.2/topics/auth/default/)

---


![beginner-friendly](https://img.shields.io/badge/beginner%20friendly-django%20project%20-green)
---


## Virtualenv & Dependencies

create a virtualenv and run requirements.txt<br/>
<b>virtualenv</b>

<pre>pip install virtualenv</pre>

<b> what is virtual environment ? </b><br/>
A virtual environment is a tool that helps to keep dependencies required by different projects separate by creating isolated python virtual environments for them. This is one of the most important tools that most of the Python developers use.
<br/>


to run requirements.txt

<pre>$ pip install -r requirements.txt</pre>

here <b>env/</b> folder contains all dependencies

## Use docker to run



## Running locally

     make database settings and connect it to your local database
    <pre>$ cd ./user_login_and_register/project </pre>
    open <b>settings.py</b> file
    <pre>
      DATABASES = {
        "default": {
            "ENGINE": "django.db.backends.mysql",
            "NAME": "iert",
            "USER": "root",
            "HOST": "localhost",
            "PASSWORD": "vinayak",
            "PORT": "3306",
            "OPTIONS": {"sql_mode": "traditional"},
        }
      }
   </pre>
   set this part according to needs.

    run migrations
  $ python manage.py migrate
  
    now, runserver
    $ python manage.py runserver
  




### Implement Token Authentication using Django REST Framework

Token authentication refers to exchanging username and password for a token that will be used in all subsequent requests so to identify the user on the server side.This article revolves about implementing token authentication using Django REST Framework to make an API. The token authentication works by providing token in exchange for exchanging usernames and passwords.

---
install django rest_framework
$ pip install djangorestframework




# Errors

## error when trying to migrate or attempting to runserver

Simply try "python3 manage.py migrate" or "python3 manage.py runserver" instead

or

Django is not installed (or installed properly)
