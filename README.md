# Django
![alt text](https://twilio-cms-prod.s3.amazonaws.com/images/django-dark.width-808.png)

## How Django Works
![alt text](https://github.com/themockingjester/Django/blob/main/images/MVT.jpeg)
###### Django use MVT (Model View Template)
###### Mode will work with data
###### view will work with logic
###### template will work with design or layout

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
###### note :- you can also use html tags with drld string


## Adding a new resource directory in django app
###### Note:- For adding any new directory as a resource(like for storing files like html,css,javascript etc) you first have to add the path of that directory in project settings.py file as an example we have created a directory below figure shows how you can add this directory as a resource

![alt text](https://github.com/themockingjester/Django/blob/main/images/adding%20resource%20folder.png)
###### Note:- here we have set a directory named templates as a resource directory and you can check image of basic project structure to see where we have made the directory named templates







## How to show a html page in django app
###### for this experiment we have added home.html page in templates directory
###### for this you have to change the the function like this way

![alt text](https://github.com/themockingjester/Django/blob/main/images/showing%20a%20html%20page.png)
<br/>
content of home.html
<br/>
![alt text](https://github.com/themockingjester/Django/blob/main/images/homedothtml.png)
<br/>
and here is the output
<br/>
![alt text](https://github.com/themockingjester/Django/blob/main/images/outpu2.png)


<br/>




## Passing a variable from python function to a html page
###### you can check the views.py , home.html and output in the figure below
![alt text](https://github.com/themockingjester/Django/blob/main/images/passing%20variables%20from%20python%20to%20html%20page.png)


## Using one html page in other html page
###### we have created a html file which will make web page of yellow color and we are importing that page in home.html page
![alt text](https://github.com/themockingjester/Django/blob/main/images/one%20html%20file%20in%20another.png)

## Getting data from user to perform some action
###### check views.py and home.html carefully and remember you have to use single quotes in GET of power function in views.py
![alt text](https://github.com/themockingjester/Django/blob/main/images/getting%20data%20from%20html%20page%20into%20python%20function.png)
###### check result.html and urls.py of App Directory carefully(since we are using a new function named power in views.py so we have to inform urls.py of App Directory about it)
![alt text](https://github.com/themockingjester/Django/blob/main/images/getting%20data%20from%20html%20page%20into%20python%20function2.png)
###### here is the output
![alt text](https://github.com/themockingjester/Django/blob/main/images/output3.png)

## How to use POST method
#### this is method is used to send data to server
###### for using post method you have to use CSRF token as we have used in home.html as shown by arrow
![alt text](https://github.com/themockingjester/Django/blob/main/images/using%20post1.png)
###### here we have shown where you can find the CSRF token in settings.py
![alt text](https://github.com/themockingjester/Django/blob/main/images/using%20post2.png)
###### output till now
![alt text](https://github.com/themockingjester/Django/blob/main/images/output3.png)

## Importing Custom Downloaded Template In Django App
###### below are the files and folders that were already present in template
![alt text](https://github.com/themockingjester/Django/blob/main/images/custom%20template1.png)
###### you can see from below image that we have put index.html in our older Directory(templates) and we have created  new directory called static for putting other static folders named css,images
![alt text](https://github.com/themockingjester/Django/blob/main/images/custom%20template2.png)
###### checkout urls.py and views.py as shown below
![alt text](https://github.com/themockingjester/Django/blob/main/images/custom%20template3.png)
###### you have to write all lines from line number 121 to line number 124  manually and in line 122 static is a folder where all the static content is available and you can have multiple directories where static data is available and you can also import them like this way as shown in image and now in line number 124 assets/ will be a folder which will automatically generated by django and here django will put all the static content loaded from different directories for its use for generating this this folder you have to type this command python manage.py collectstatic
![alt text](https://github.com/themockingjester/Django/blob/main/images/custom%20template4.png)
###### see line 1,8,14 carefully and from 8 and 14 we can conclude that we have to put the name of path of static file in {% static %} 
![alt text](https://github.com/themockingjester/Django/blob/main/images/custom%20template5.png)



### Basic Commands



## Creating New Project
###### django-admin startproject projectname

## Running Server
###### pythonmanage.py runserver

## Creating New App
###### python manage.py startapp nameoftheapp
