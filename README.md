# How to build a Django web project
Huge chunks of code come from the tutorials of [https://www.pythonprogramming.net](https://www.pythonprogramming.net)


## Generate the project structure
 * run ``` django-admin startproject <projectname>``` to generate the project structure
 * hide the generated secrete key
 * run ```python3 manage.py runserver``` to check everything is working
 
Now you can look at the django template in your browser by calling your local host.  
Your localhost is usually  127.0.0.1 and django uses port 8000 for the development server

## Generate the first app

 * run ```python3 manage.py startapp <appname>``` to generate the apps structure
 * add the app's name to the app list in the settings.py file
 * add the app's urls to urls.py
 You probably want to use include, so import it!
 * run server again and check if the app displays the content on ```127.0.0.1:8000/<appname> ```

## Folder Structure
Django collects all files from the directories called static and templates. So you should give the file unique names or use subdirectories.

## Style sheets
Easiest is to download cascading stylesheets(css) from [bootstrap](https://getbootstrap.com/) and save the template in a static directory.
But be aware, static file are public!