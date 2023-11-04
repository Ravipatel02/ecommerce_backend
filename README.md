# ecommerce_backend

**
###How to run in local

src/main/resources/application.properties.
Change the Application Properties (E.g. username/password of DB) present in resources/application.properties according to your local mysql-server.
Example:
 spring.datasource.url=jdbc:mysql://localhost:3306/DATABASE_NAME  Note : First create databas in MY_SQL (database name :ecommerce )
 spring.datasource.username=root                                                                              
 spring.datasource.password=root                                      
 spring.jpa.hibernate.ddl-auto=update                                                                                                                                                 
 spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver                                                           



To run the application, automaticaly created all table;
example :
1-user
2 - category
3 - product
4 - cart
5 - wishlist

show on

Hit Url :

USER API :

Sign up :

url : (postMapping)  http://localhost:8080/user/signup 
pass to data this formate -
{
        "firstName": "ramram",
        "lastName": "Patel",
        "email": "ram@gmail.com",
        "password": "ram0929"
}

Sign In :
url: (PostMapping)  http://localhost:8080/user/signIn

hit josn farmet:
{
    "email":"ram@gmail.com",
    "password":"ram0929"
}

Result :

{
    "status": "success",
    "token": "a28429b6-7f72-4c91-be3c-d1625658c2cf"
}

Get ALL USER :
GetMapping (url) http://localhost:8080/user/all ? token = pass to token
Note : need Token
Eample : http://localhost:8080/user/all?token=e8d2b831-5c9e-4e28-a66c-83220ff88022


**
