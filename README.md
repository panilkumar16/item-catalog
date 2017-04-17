# Catalog App (Categories with Items)
The Catalog App can be used by users in world to view different Categories and its respective items.  It can have sports categories and items, or any as you prefer.

Users can view all the Categories and Items.  Logged in users can add, edit, delete their own Categories and Items.  Can view who added a specific Category.

Users can login using secure OAuth login providers like Google and Facebook.

The Catalog App can contain list of Categories.  Each Category has list of items.  Each item has title, description, date created, and which category it belongs to.

The Catalog App is a application developed in HTML, CSS, JavaScript, Bootstrap Framework, Ajax, jQuery, JSON, RESTfull APIs, Python, Flask Framework, Database with SQLAlChemy Python Module.


# Table of Contents
1. [Author](#author)
2. [Instructions on running the project](#instructions)
3. [Directory Structure](#directory-structure)


<br><br>
### <a name="author"></a>1. Author

Anilkumar P
<br>
<br>
<br>

### <a name="instructions"></a>2. Instructions on running the project

1) Make sure you install Virtual Box and Vagrant for your Operating System.  We need this
   because we will be using a Virtual Machine to run this project
   See below links for downloading and installing:
   https://www.virtualbox.org/wiki/Downloads
   https://www.vagrantup.com/downloads.html
2) If you are using MacOS or Linux you can use your terminal to execute the below commands.
   If you are using Windows OS download Git Bash to execute below commands.  You can download
   and install Git Bash at https://git-scm.com/download/win
3) First unzip the zip file to fullstack
4) In that unzipped director you see directories and files as listed in section 3.
5) Open the fullstack folder where ever you downloaded on your system and
   go to path fullstack/vagrant and execute below commands:

   ```
   $ vagrant up

   ```

   This will take time.  After completion it will give the message.
   You can connect to vagrant VM with  below command:

   ```
   $ vagrant ssh

   ```

6) Go to the project directory to create the database, tables, and to launch the application:
   ```
   $ cd /vagrant/catalog
   $ python database_setup.py
   $ python application.py

   ```

7) Go to your browser and go to url http://localhost:8000/ to view the application on your browser.  Click login button to login with secure OAuth providers Google or Facebook to view and create your Categories.


<br>
<br>
<br>

### <a name="directory-structure"></a>3. Directory Structure

```
-vagrant
   -directory containing below directories
   .vagrant
      - directory required for vagrant functionality and VM
   catalog
      - files:
         README.md - this readme file
         database_setup.py to create database and tables
         application.py python program for catalog application
         client_secrets.json configuration file for Google OAuth login
         fb_client_secrets.json configuration file for Facebook OAuth login
         Other files you can leave as it is
      - static directory:
        bootstrap-3.3.7-dist directory for Bootstrap framework
        bootstrap_custom.css for customization of bootstrap for this app
      - template directory:
        Contains all html files for Web Application Pages as below:
            catalog.html
            deleteCategory.html
            deleteItem.html
            editCategory.html
            editItem.html
            flash_message.html
            footer.html
            header.html
            items.html
            login.html
            main.html
            newCategory.html
            newItem.html
            oneItem.html

   Other directories and files you can leave as it is

```
