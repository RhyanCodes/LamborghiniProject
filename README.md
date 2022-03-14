# Lamborghini Project
A website where you can order custom Lamborghini vehicles.
  1. The website layout and design was made using HTML & CSS.
  2. Python was used to import user input into a PostgreSQL database.
  3. Psycopg2 was used as the PostgreSQL database adapter.
  4. Flask-Sqlalchemy was also used for connection with PostgreSql.

# Start Project Locally
First, make sure to install the latest version of Python and PostgreSQL. Then, create a project folder and import the project files. Next, open Command Prompt(or Terminal) and ```cd``` into the project folder. Create a folder within the project folder called templates and another folder called static. Import all HTML files into the templates folder and CSS, MP4, and PNG files into the static folder.

To start and run locally:
  1. Install Virtual Environment under the project folder in the command prompt(terminal)
  ```
  pip install virtualenv
  ```
  2. Specify the folder to install virtual environment in. This will create a folder called 'virtual'.
  ```
  python –m venv virtual 
  
  python –m virtualenv virtual (If on Mac)
  ```
  3. ```cd``` into the 'virtual' folder and then ```cd``` again into the 'Scripts' folder and type activate. This will trigger the virtual environment.
  ``` 
  C:\Users\aj\projectfolder>virtual\Scripts\activate
  ```
  4. Under the projecct folder, install Flask. 
  ```
  (virtual) C:\Users\aj\projectfolder>pip install flask
  ```
  5. Next, install psycopg2.
  ```
  (virtual) C:\Users\aj\projectfolder>pip install psycopg2
  ```
  6. Then, install Flask-SQLAlchemy.
  ```
  (virtual) C:\Users\aj\projectfolder>pip install Flask-SQLAlchemy
  ```
  7. Open PgAdmin and create a database called 'orders'. Make the password of the database unique and change the 'xxxx' in line 5 of 'app.py' to your new unique password 
  ![image](https://user-images.githubusercontent.com/77405871/158089236-421138be-ddf2-4c86-b012-bbe1631de41b.png)
  
  8. In Command Prompt(Terminal) type in ```python```
  ```
  (virtual) C:\Users\aj\projectfolder>python
  ```
  9. Once you see ```>>>```, type in ```>>> from app import db```
  ``` 
  >>> from app import db
  ```
  10. After, type in ```>>> db.create_all()``` and then refresh the database and check the table.
  ```
  >>> db.create_all()
  ```
  11. Exit out of python by typing ```exit()``` and type ```app.py```
  ```
  >>> exit()
  (virtual) C:\Users\aj\projectfolder>app.py
  ```
  12. Go to localhost:5000 in your web browser of choice and the website will be running. Click on 'Order Now' and then input your data into the order form. Once you click   'Submit', you will see the Thank You page. In PgAdmin, right click on the table called 'lamborghini_orders' and click on 'Query Tool'. Then, type in ```select *from lamborgini_orders``` in the Query Tool and hit the Play button to see the order data. 
  ![image](https://user-images.githubusercontent.com/77405871/158090490-fddd675b-71e8-443a-9c04-65b623612678.png)

  
# Website 
1. Welcome Page 

  ![image](https://user-images.githubusercontent.com/77405871/158090013-9f2fb779-a3b5-4137-ac3f-75821cc3d4af.png)

2. Custom Ordering Page

  ![image](https://user-images.githubusercontent.com/77405871/158091030-cf9227dd-3ef3-4cf5-b5ad-cec406604b0f.png)

3. Order Confirmation Page 

  ![image](https://user-images.githubusercontent.com/77405871/158091128-68b4a4cc-6d94-4ed6-a299-068b7af3fd69.png)

