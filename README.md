# E-Commerce

    An e-commercial website

# Back End Technologies:

- Java JDK 17
- Java Framework: Spring Boot 2.4.2
- Dependencies: Security, JPA, Web, Validation Api, MySQL connector, starter test, security test...
- Database: MySql
- IDE: Intelij

# Database Design:

![picture alt](/1.png "Database")

# Spring Boot Architecture:

- Controller -> Service -> DAO (Repository) -> (data) -> Service -> Controller -> Web/Web Client.

# Checking All API Endpoints Using Postman:

- POST http:localhost:7090/api/addUser : 200 OK

![picture alt](/3.png "Add User")

- GET http://localhost:7090/api/admin/findAllUsers : 200 OK

::: warning
_This is security risk! With the url api, one can obtain sensity list of all customers!!! This is the case where I will add JWT to stop this from happening._
:::

![picture alt](/4.png "Add User")

# JWT implementation (JSON WEB TOKEN) (To be implemented)

- We use JWT for API authorization. Whenever user want to access an API, you will need to provide JSON web token to the server:
- There are 3 parts: Header - Payload (information about the owner of the token) - Signature.
- One application communcation to another application will also need this token.
- Testing http://localhsot:7090/api/login/user
  with test case header as: {"mobile": 9164725749, "password": "testpassword"}
  will return payload user information and a user token as following:
  ![picture alt](/2.png "Database")
