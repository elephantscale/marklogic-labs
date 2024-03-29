# Create a new Databsase

In this lab we will practice the Database creation. 


### Follow the following steps to create a new database:

* Log into the Admin Interface in a browser. It is on port 8001 of the host in which MarkLogic is running. From your windows machine, http://18.222.133.222:8001 (In this case the EC2 instance IP is 18.222.133.222. Accordingly you neee to change it as per your EC2 instance IP).

* You will be prompted to log in with your admin username and password

    <img src="../images/Config_4.jpg" style="width:80%;"/> <!-- {"left" : 0.26, "top" : 1.45, "height" : 6.17, "width" : 9.74} -->

* Click the Databases icon in the left tree menu

    <img src="../images/db_1.jpg" style="width:80%;"/> <!-- {"left" : 0.26, "top" : 1.45, "height" : 6.17, "width" : 9.74} -->

* Click the Create tab at the top right. The Create Database page displays:

    <img src="../images/db_2.jpg" style="width:80%;"/> <!-- {"left" : 0.26, "top" : 1.45, "height" : 6.17, "width" : 9.74} -->

* Enter the name of the database. This is the name the system will use to refer to this database.

    <img src="../images/db_3.jpg" style="width:80%;"/> <!-- {"left" : 0.26, "top" : 1.45, "height" : 6.17, "width" : 9.74} -->

* Select a security database to be associated with this database. We recommend selecting Security as the security database.

* Select a schema database to be associated with this database. We selected Schemas as schema database.

    <img src="../images/db_4.jpg" style="width:80%;"/> <!-- {"left" : 0.26, "top" : 1.45, "height" : 6.17, "width" : 9.74} -->

* You may leave the rest of the parameters unchanged or set them according to your needs

* Click OK:

* Database successfully created

    <img src="../images/db_5.jpg" style="width:80%;"/> <!-- {"left" : 0.26, "top" : 1.45, "height" : 6.17, "width" : 9.74} -->

* You can now attach forests to the database. Creating a database is a hot admin task.