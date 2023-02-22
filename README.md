# Spring-Hibernate-AOP App
<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Yaroslav-by/spring-hibernate-aop">
    <img src="https://download.logo.wine/logo/Spring_Framework/Spring_Framework-Logo.wine.png" alt="Logo" width="300" height="200">
  </a>

<h3 align="center">Spring Hibernate AOP App</h3>

  <p align="center">
    Simple practice app that uses Spring framework, hibernate, TomCat.
    <br />
    <br />
    <a href="https://github.com/Yaroslav-by/spring-hibernate-aop">View Demo</a>
    ·
    <a href="https://github.com/Yaroslav-by/spring-hibernate-aop/issues">Report Bug</a>
    ·
    <a href="https://github.com/Yaroslav-by/spring-hibernate-aop/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[<a href="https://ibb.co/4TtDJmx"><img src="https://i.ibb.co/r60Lv7J/image.png" alt="image" border="0" /></a>](https://github.com/Yaroslav-by/spring-hibernate-aop)

This project uses Spring framework, Hibernate, TomCat, MySQL Database.
<br> <br>
The application uses the DAO(Data Access Object) principle to communicate the java with the database. 
The controller is connected to the service, the service is connected to the DAO, the DAO is connected to the database via hibernate.
On the main page we can see all Employees from our Database. There are ADD, UPDATE and DELETE buttons. ADD button can add new Employee to Database.
UPDATE button can change information about Employee. DELETE button delete Employee from the Database and from the project.
<br><br>
Also, there is a simple implementation of AOP. It writes information about beginning and ending of each methods to console.

<br>


<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* Java
* Spring framework
* MySQL Database
* TomCat

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/Yaroslav-by/spring-hibernate-aop
   ```
2. Create database in MySQL database.
3. Connect database with Java via applicationContext.xml.
```Java
    <bean id="dataSource" class="com.mchange.v2.c3p0.ComboPooledDataSource"
          destroy-method="close">
        <property name="driverClass" value="com.mysql.cj.jdbc.Driver" />
        <property name="jdbcUrl" value="jdbc:mysql://localhost:3306/my_db?useSSL=false&amp;serverTimezone=UTC" />
        <property name="user" value="{Your username}" />
        <property name="password" value="{Your password}" />
    </bean>
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage
By click on ADD button you can see this window. You can type information about new Employee and add him to Database.<br>
<a href="https://ibb.co/pLZpkrL"><img src="https://i.ibb.co/NypzGny/image.png" alt="image" border="0" /></a><br>
Here is a result.<br>
<a href="https://ibb.co/P9dnJT7"><img src="https://i.ibb.co/RBqmthx/image.png" alt="image" border="0" /></a>
<br><br>
By click on Update button you can see this window. You can type new information about existing Employee and update him in Database.<br>
<a href="https://ibb.co/T4gHjtp"><img src="https://i.ibb.co/dP5QCD1/image.png" alt="image" border="0" /></a> <br>
Here is a result. <br>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/dtm6MXk/image.png" alt="image" border="0" /></a>
<br><br>
DELETE button just delete existing Employee from the Database.
<br><br>
Here is an example of AOP realisation in console by click on UPDATE button.<br>
<a href="https://ibb.co/fNJKdhW"><img src="https://i.ibb.co/mypY5LK/image.png" alt="image" border="0" /></a>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [+] Show all Employees
- [+] Annotation Service
- [+] Add new Employee
- [+] Update Employee
- [+] Delete Employee
- [+] Simple logging in console via AOP.
- [-] Search Employee by name, salary, department.
- [-] Usage of Spring boot framework.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Yaroslav Salnikov - asgen-yaroslav@mail.ru

Project Link: [Spring Hibernate AOP App](https://github.com/Yaroslav-by/spring-hibernate-aop)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
