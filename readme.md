# Event Planner App 

#### Collaborators
Adam Paslawski\
Chelsea Mitchell\
Warren Liu\
Insung Youn\
Fenil Patel\
Zexi Lv\
Daniel Dizon

## Additional Features:
* We implemented a GUI with JavaFX, with an inbuilt MVC model, replacing the original command line 
interface. This command line interface has been kept in the classes ControllerMainLoop and ControllerMenu, 
but have not been updated or fixed for phase 2. Controller presenter separation was achieved through JavaFX's architecture.
* We used an AWS RDS MySQL DB and connected to it via a Java.SQL Gateway class. The AWS RDS mySQL database provided for total coverage and storage of our core entities and data.
* For an additional user type, we implemented an Admin, who can remove 
or cancel events, or completely delete messages
* We also implemented a feedback system that provides feedback for the app anonymously
that demonstrates the extendability of our program, which provides a data export for actors who need it.
* Packaging wise, we used a clean architecture layer packaging system except the GUI, which we believed was best to be packaged separate to the rest of the program as its role is very focused.

## To setup database access on your machine
You must enable the driver for the MySQL JDBC database connection.
* An example driver that works is "mysql:mysql-connector-java:8.0.11"

## To run the program:

* To run the program, navigate to /src/GUI/DisplayMain.java
* Execute the run through an IDE or through the command line
* Our program's access point is through DisplayMain

#### Key Design Choices:
* For many of our classes, to follow a MVC architecture 
or use functionality, we had to use dependency 
inversion.
* Dependency injection in places helped us encapsulate
code and speed up development
* We packaged by Clean Architecture layer in order to 
enforce dependency rules and invert when necessary.
* Design patterns were only introduced when they did 
not overcomplicate the code or provide for 
useless functionality.

Yours Truly, \
Group 0162
