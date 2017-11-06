<link rel='stylesheet' href='./web/swiss.css'/>

# Sprint 4: Spring Data (JPA) and Spring Security 

In this sprint, we are going to focus on how to implement two important aspects of web applications:
* persistence using a relational database (MySQL): we will generate the database automatically from our POJOs; and
* security.

We are going to use agile software development based on test-driven development and behaviour-driven development, as explained in Sprint 2.


## The Sprint Goal (assessed coursework)

The goal of this Sprint is to test a web application: 

* :dart: [mini project worksheet](./worksheet.md) (the link will not work until the worksheet is released):
  * **marks: 100, weight: 20%** of overall mark
  * checkpoint: **Thursday 30th November, 9 am, weight 10% of sprint 3**
  * release: **Thursday 7th December, 9 am, weight 90% of sprint 3**
  * this assessment is **individual** and you should not work with other students in your solution, which is penalised as [a form of plagiarism (namely, collusion)](https://campus.cs.le.ac.uk/ForStudents/plagiarism/DoAIF.pdf)


## Week 1. Spring Data 

### What to focus on during the following week?

#### JPA

* The object relational mapping problem
* What is JPA?
* What is an Entity?
* Spring MVC architecture
  * service layer
  * repository layer
* JPA/Hibernate configuration: what options are available for initialising a database `hbm2ddl`
* **JPA annotations** 
  * `@Entity` 
  * `@Table`
  * `@Id`
  * `@GeneratedValue`
  * `@Column`
  * `@Column`
  * Join types: 
    * `@OneToOne`
    * `@OneToMany`
    * `@ManyToOne`
    * `@ManyToMany`
    * configuration
      * unidirectional/bidirectional/cascasde
      * Fetch type: lazy/eager
* What is Spring Data JPA?   
   
#### Spring Data JPA
* What is a Spring JPA repository?
* What can we do with a Spring JPA repository?
  * How to use CRUD operations?
* What is the Query DSL?
  * Query method syntax basics
  * Query method return types
  * Keywords: use as reference (remember that most of these keywords correspond to clauses that can be used in a SQL SELECT statement)

### Pluralsight resources

The approach that we are using in CO2006 for configuring Spring MVC apps is based on Java configuration (as opposed to XML configuration as done in the Pluralsight tutorial), to be discussed in the lecture and exercises.

####  Spring, JPA and Hibernate

Some differences with the Pluralsight tutorials:
  * The tutorial uses Spring Validation, whereas we used error handling with exceptions
  
This tutorial builds on the case study used in the tutorial [Introduction to Spring MVC](https://app.pluralsight.com/player?course=springmvc-intro), the project `Fitness Tracker` and the examples can be migrated to Gradle/Java configuration using the [migration guide from Maven to Gradle](https://github.com/uol-inf/CO2006-16-17/blob/master/sprint2/MigratingToGradle.md).  Watch the following tutorials:
  * :movie_camera: [Introduction](https://app.pluralsight.com/player?course=spring-jpa-hibernate&author=bryan-hansen&name=springjpa-m1-intro&clip=0&mode=live)
  * :movie_camera: [MVC Demo](https://app.pluralsight.com/player?course=spring-jpa-hibernate&author=bryan-hansen&name=springjpa-m2-scaffold&clip=0&mode=live): the project `Fitness Tracker`
  * :movie_camera: [Architecture](https://app.pluralsight.com/player?course=spring-jpa-hibernate&author=bryan-hansen&name=springjpa-m3-architecture&clip=0&mode=live): revisiting architectural design with more emphasis on persistence (databases)
  * :movie_camera: [Overview of JPA and creating your first entity](https://app.pluralsight.com/player?course=spring-jpa-hibernate&author=bryan-hansen&name=springjpa-m6-jpa&clip=0&mode=live)
  * :movie_camera: [JPA annotations and how to use them](https://app.pluralsight.com/player?course=spring-jpa-hibernate&author=bryan-hansen&name=springjpa-m7-jpaannotation&clip=0&mode=live)
    * **skip** 
      * JPQL/JPQL demo
      * OpenEntityManagementInViewFilter
      * Lazy Initialization Fix Demo
      * Projection/Projection Demo
      * Named queries/named queries demo

#### Spring Data JPA
  * :movie_camera: [Getting Started](https://app.pluralsight.com/player?course=spring-data-jpa-getting-started&author=dan-bunker&name=spring-data-jpa-getting-started-m1-intro&clip=0&mode=live)
    * introduction to Spring Data JPA
    * case study: guitar project (uses Maven and Java configuration): use the [migration guide from Maven to Gradle](https://github.com/uol-inf/CO2006-16-17/blob/master/sprint2/MigratingToGradle.md) 
  * :movie_camera: [Spring Data Repositories](https://app.pluralsight.com/player?course=spring-data-jpa-getting-started&author=dan-bunker&name=spring-data-jpa-getting-started-m2-repositories&clip=0&mode=live)
  * :movie_camera: [QueryDSL](https://app.pluralsight.com/player?course=spring-data-jpa-getting-started&author=dan-bunker&name=spring-data-jpa-getting-started-m3-queries&clip=0&mode=live)

### Exercises (formative coursework)
* :computer: [Spring Data Exercise](./SpringData_ex01/readme.md)
  * Configuring a database connection
  * Defining JPA annotations
  * Using Spring Data repository interfaces
  * :computer: [solution](./SpringData_ex01_solution/) (this link will be enabled when the solution is released)
* :computer: [Fitness tracker examples](https://app.pluralsight.com/library/courses/spring-jpa-hibernate/exercise-files) (Excercise files)
* :computer: [Guitar company examples](https://app.pluralsight.com/library/courses/spring-data-jpa-getting-started/exercise-files) (Excercise files)

Solutions to exercises will be posted under this folder on GitHub as projects with the name `${ExerciseName}_solution`.  

## Week 2. Spring Security 

### What to focus on during the following two weeks?
* Architecture of a secure Spring MVC web app
  * Authentication
  * Authorization
* User storage
* Password encryption
* Access control lists (ACLs)
* Secure communication
  * HTTPS
  * Man in the middle attack
  * Certificates

### Pluralsight resources
* :movie_camera: [Introduction to Spring Security](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m1-intro&clip=0&mode=live)
* :movie_camera: [Scaffold application](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m2-scaffold&clip=0&mode=live)
  * Building on the `Fitness Tracker` application used in previous tutorials
  * Some differences with what we are using are:
    * We are using containerless applications where the web server is embedded into our applications by using Spring Boot. Use the view `Boot Dashboard` instead of the view `Servers` to run your web app within the STS.
    * We are using Gradle instead of Maven and Java configuration instead of XML configuration. See the usual [migration guide from Maven to Gradle](https://github.com/uol-inf/CO2006-16-17/blob/master/sprint2/MigratingToGradle.md) for reusing the examples provided.
* :movie_camera: [Securing your Spring MVC Application](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m3-first-app&clip=0&mode=live)
  * replace most of the XML configuration for what we will discuss in the lecture
* :movie_camera: [User storage](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m4-user-storage&clip=0&mode=live)
* :movie_camera: [Spring Security Client Integration](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m5-client&clip=0&mode=live)
  * we are going to configure authentication and access control using the Spring Security DSL as shown in the lecture
* :movie_camera: [Password Storage](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m6-passwords&clip=0&mode=live)
* :movie_camera: [Customizing Spring Security](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m7-customizing&clip=0&mode=live)
  * we are going to customize security using the Spring Security DSL as shown in the lecture
* :movie_camera: [Forcing the use of HTTPS](https://app.pluralsight.com/player?course=spring-security-fundamentals&author=bryan-hansen&name=springsec-fundamentals-m9b-https&clip=0&mode=live)

### Exercises (formative coursework)
* :computer: [Spring Security Exercise](./SpringSecurity_ex01/readme.md): base code in the project `SpringMvc_product_sec` for implementing the security layer
  * :computer: [solution](./SpringSecurity_ex01_solution/) (this link will be enabled when the solution is released)
* :computer: [Fitness tracker examples](https://app.pluralsight.com/library/courses/spring-security-fundamentals/exercise-files) (Exercise files)

Solutions to exercises will be posted under this folder on GitHub as projects with the name `${ExerciseName}_solution`.

## Final test (assessed coursework)

* :dart: **Final Test (covering sprints 2, 3 and 4): Wednesday 13th December**
  * Group A: 14:00-15:00
  * Group B: 15:00-16:00
* Revision: you may want to revisit these in preparation for the test in January
  * Introduction Spring MVC: [learning check quiz](https://app.pluralsight.com/library/courses/springmvc-intro/learning-check) 
  * Introduction to TDD: [learning check quiz](https://app.pluralsight.com/library/courses/java-testing-introduction/learning-check)
  * A sample test can be found [here](https://blackboard.le.ac.uk/webapps/assessment/take/launchAssessment.jsp?course_id=_1807_1&content_id=_1451990_1)
  * The **revision session** will be on **Tuesday 12th December, 16:00, in ENG LT2** (note the change of room)



## Jargon buster <a name="jargon"></a>

| term  | definition | source |
|-------|------------|--------|
| Repository | CRUD interface for a database table | [Working with Spring Data Repositories](http://docs.spring.io/spring-data/data-commons/docs/1.6.1.RELEASE/reference/html/repositories.html) |
| Domain class | Plain old class modelling data, which will usually be mapped to a table | |
| MySQLWorkbench | GUI for MySQL database server | [http://mysqlworkbench.org](http://mysqlworkbench.org) |  
| Asset | System resource that has value to one or more stakeholders. Ex: a system component, data, system memory, processor capacity | [Sommerville9,11.4] |   
| Exposure | Possible loss or harm to a computing system. Ex: loss or damage to data, loss of time and effort invested in recovering the system | [Sommerville9,11.4] |  
| Vulnerability | Weakness in a system that may be exploited to cause loss or harm. Ex: policy of password renewal is too fast paced and requires complex characters | [Sommerville9,11.4] |  
| Attack | Exploitation of a system’s vulnerability. Ex: stealing a password. | [Sommerville9,11.4] |  
| Threat | Circumstances under which an attack can be performed. Ex: employees write down their passwords. | [Sommerville9,11.4] |  
| Security control | Protective measure to reduce a system’s vulnerability. Ex: encryption to reduce vulnerability of a weak access control system. |[Sommerville9,11.4] | 
| Public key certificate | Electronic document used to prove the ownership of a public key | [wikipedia](https://en.wikipedia.org/wiki/Public_key_certificate) |
| HTTPS | Protocol for secure communication over a computer network | [wikipedia](https://en.wikipedia.org/wiki/HTTPS) |
| Man-in-the-middle attack | Attack used to sniff information from a communication between two systems. | [OWASP](https://www.owasp.org/index.php/Man-in-the-middle_attack) | 


## Additional resources (for reference)

These are pointers to official documentation in case you need to expand your knowledge when implementing the mini project (part II):
* [SQL (w3schools tutorial)](http://www.w3schools.com/sql/)

### Spring Data

* [Nicholas S. Williams. Professional Java for Web Applications. Addison-Wesley. 2014.](http://readinglists.le.ac.uk/items/51133F43-7D8E-3A7B-952C-6DA5DC168B73.html?referrer=%2Flists%2FAE79369B-4CED-C912-2150-5BD837030B59.html%23item-51133F43-7D8E-3A7B-952C-6DA5DC168B73) (link to ebook on Library catalogue). Chapters 19-23.
* [Official documentation about Spring Data](http://docs.spring.io/spring-data/jpa/docs/current/reference/html/)

### Spring Security

* [Nicholas S. Williams. Professional Java for Web Applications. Addison-Wesley. 2014.](http://readinglists.le.ac.uk/items/51133F43-7D8E-3A7B-952C-6DA5DC168B73.html?referrer=%2Flists%2FAE79369B-4CED-C912-2150-5BD837030B59.html%23item-51133F43-7D8E-3A7B-952C-6DA5DC168B73) (link to ebook on Library catalogue). Chapters 25-26.
* [Official documentation about Spring Security](http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/)






