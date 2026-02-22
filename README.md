# 🥘 Food Order Website 

# ⚙️ Technology Used
1. HTML5
2. CSS3
3. Core/Procedural PHP programming language
4. MySQL Relational Database


# 🧰 Features
1. Visitors and users can browse all food categories and available items on the website.
2. Users can easily place orders through the online ordering system.
3. The admin can manage administrators, categories, and food items.
4. The admin can monitor, manage, and track food orders and delivery status.


# Screenshots
<img width="876" height="437" alt="image" src="https://github.com/user-attachments/assets/72790bdf-048b-4b73-9b47-1fd82fa093f0" />

<img width="238" height="224" alt="image" src="https://github.com/user-attachments/assets/c043e3ee-09a3-4567-bf4e-bc9473f8d930" />

<img width="840" height="456" alt="image" src="https://github.com/user-attachments/assets/66102e83-a1bd-4413-ad35-b7a3d3a834a9" />



## 📖  How to Download the Project and Run on your PC?

### Pre-Requisites:

1. Download and Install XAMPP

[Click Here to Download](https://www.apachefriends.org/index.html)

2. Install any Text Editor (Sublime Text or Visual Studio Code or Atom or Brackets)

### Installation

1. Download as as Zip or Clone this project
2. Move this project to Root Directory
```
Local Disc C: -> xampp -> htdocs -> 'this project'
```
*Local Disk C is the location where xampp was installed*

3. Open XAMPP Control Panel and Start 'Apache' and 'MySQL'

4. Import Database

a. Open 'phpmyadmin' in your browser
b. Create a Database
c. Import the SQL file provided with this project

5. Make Changes to settings

Go to 'config' folder and Open 'constants.php' file. Then make changes on following constants
```php
<?php 
//Start Session
session_start();

//Create Constants to Store Non Repeating Values
define('SITEURL', 'http://localhost/food-order/'); //Update the home URL of the project if you have changed port number or it's live on server
define('LOCALHOST', 'localhost');
define('DB_USERNAME', 'root');
define('DB_PASSWORD', '');
define('DB_NAME', 'food-order');
    
$conn = mysqli_connect(LOCALHOST, DB_USERNAME, DB_PASSWORD) or die(mysqli_error()); //Database Connection
$db_select = mysqli_select_db($conn, DB_NAME) or die(mysqli_error()); //SElecting Database 

?>
```

6. Now, Open the project in your browser.

