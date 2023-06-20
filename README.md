# taxi-service
## Description

Taxi service is project created while practice skills in different technologies like Servlets.

### Features
- driver registration
- driver authentication
- create/remove/update a car
- create/remove/update a driver
- create/remove/update a manufacturer
- display list of the manufacturers
- display list of cars
- display list of cars for logged driver
- display list of manufacturers

### Project structure:
- controller:
    - package has classes that process responses and requests from the client side
- dao:
    - data access object package has classes that described CRUD operation
- exception:
    - implemented two custom exception - checked and unchecked
- lib:
    - package has custom annotation and class implementation Injector
- model:
    - packaged described models for the three objects: Car, Driver and Manufacturer
- service:
    - described classes for interaction with classes from the dao package and implemented authentication logic
- util:
    - package has a class that described connection with database
- webapp.filter: package has a class that implemented interface filter:
    - **init()** method initialize allowedUrl set
    - **doFilter()** method implemented filter logic
- resources: init_db.sql
- web:
    - web.xml: servlets configurations
    - WEB-INF/views: described jsp pages
### Technologies:
- JAVA 11
- Tomcat 9.0.75
- Maven
- Dependency Injection
- Filter
- MySQL
- JDBC
- JCP
- Git
- HTML
- CSS
### How to run project:
- Download and set up: tomcat 9.0.75, Intellij Idea ultimate, mysql and java 11
- Open the project and run the script **init_db.sql**
  (location: _src/main/resources_) in mysql.
- Set up your database connection settings in the file **ConnectionUtil** (location: _src/main/java/taxi/util_). You should set up: URL, USERNAME, PASSWORD, JDBC_DRIVER
- Configure tomcat and run the project