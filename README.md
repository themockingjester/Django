# Django
![alt text](https://twilio-cms-prod.s3.amazonaws.com/images/django-dark.width-808.png)
## Basic Project Structure

![alt text](https://github.com/themockingjester/Django/blob/main/images/project%20structure.png)

## Directory(automatically created by project) structure

![alt text](https://github.com/themockingjester/Django/blob/main/images/structure%20of%20project%20created%20folder.png)


## App Directory Structure
###### Note:- here in this stucture file named urls.py is created by us
###### models.py used to hold data
###### tests.py used for tesing our app
###### views.py used for sending request
![alt text](https://github.com/themockingjester/Django/blob/main/images/app%20folder%20structure.png)

### Note:- if you want your user can use your app(including you also) then you have to add urls.py of App Folder inside urls.py of Project Folder like this way as shown in image below
![alt text](https://github.com/themockingjester/Django/blob/main/images/accessing%20apps%20urls.png)
###### in above image line:- path('',include('myapp.urls')), tells computer hey you have to go to urls.py of the App henc user can access the app


## Basic Content of urls.py in App's Directory
###### Note: this file will be created by us django donot make it for us!
![alt text](https://github.com/themockingjester/Django/blob/main/images/urlsdotpy.png)

###### 1) in path function we used empty string because it denotes homepage
###### 2) you can see in name parameter of path function we have written home but we can write other things also like index.html
###### 3) you can see we have written views.home in path function so we have to make a function named home in views.py file of the App Folder
#### below is shown how to write home function
![alt text](https://github.com/themockingjester/Django/blob/main/images/views.png)
##### output till now
![alt text](https://github.com/themockingjester/Django/blob/main/images/output1.png)
### Basic Commands


## Creating New Project
###### django-admin startproject projectname

## Running Server
###### pythonmanage.py runserver

## Creating New App
###### python manage.py startapp nameoftheapp
