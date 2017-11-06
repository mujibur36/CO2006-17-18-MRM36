<link rel='stylesheet' href='./web/swiss.css'/>

# Sprint 3: Quality Assurance (Test-Driven Development)

In the previous sprint, we started working in quality assurance of web apps by implementing fault prevention strategies using the validation library of the Spring framework.

In this sprint, we are going to focus on testing Spring web apps using agile testing based on test-driven development and behaviour-driven development.


## The Sprint Goal (assessed coursework)

The goal of this Sprint is to test a web application: 

* :dart: [mini project worksheet](./worksheet.md) (the link will not work until the worksheet is released):
  * **marks: 100, weight: 20%** of overall mark
  * checkpoint: **Thursday 9th November, 9 am, weight 10 % of sprint 3**
  * release: **Thursday 16th November, 9 am, weight 90 % of sprint 3**
  * this assessment is **individual** and you should not work with other students in your solution, which is penalised as [a form of plagiarism (namely, collusion)](https://campus.cs.le.ac.uk/ForStudents/plagiarism/DoAIF.pdf)


## Week 1. Test-driven development

### What to focus on during this week?
* What is software testing? 
  * What is the advantage of **automated testing** with respect to manual testing?
  * What are the main types of testing activities?
    * unit testing
    * integration testing (aka aggregate testing) 
    * system testing (aka functional testing or end-to-end testing)
* JUnit
  * test structure: **given/when/then** clauses
  * understand differences between: **exception** vs **error** vs **failure**
* Tests as executable documentation
  * good coding practices:
    * naming conventions
    * test behaviour
    * DRY
    * diagnostics messages
  * @Before/@After annotations
  * **Hamcrest** library for implementing oracles (assertions)
* **Test-driven development** (TDD)
  * iterative workflow: **RED/GREEN/REFACTOR** (failing test/passing test/refactor code)
  * triangulation process: from requirement (test specification) to implementation 
    
### Pluralsight resources
* [Introduction to testing in Java](https://app.pluralsight.com/library/courses/java-testing-introduction/table-of-contents)
  * :movie_camera: [Introduction](https://app.pluralsight.com/player?course=java-testing-introduction&author=richard-warburton&name=java-testing-introduction-m1&clip=0&mode=live)
  * :movie_camera: [Testing code](https://app.pluralsight.com/player?course=java-testing-introduction&author=richard-warburton&name=java-testing-introduction-m2&clip=0&mode=live)
    * for running tests from command line, use Gradle with the command `./gradlew test` (or in windows: `gradlew.bat test`)
  * :movie_camera: [Writing good tests](https://app.pluralsight.com/player?course=java-testing-introduction&author=richard-warburton&name=java-testing-introduction-m3&clip=0&mode=live)
  * :movie_camera: [Introducing Test-Driven Development](https://app.pluralsight.com/player?course=java-testing-introduction&author=richard-warburton&name=java-testing-introduction-m4&clip=0&mode=live)
  
### Exercises (formative coursework)
* :computer: From Pluralsight tutorial [Introduction to testing in Java](https://app.pluralsight.com/library/courses/java-testing-introduction/table-of-contents), under tab `Exercise files`
  * check exercises in folders `2-java-testing-introduction-m2-exercise-files` to `4-java-testing-introduction-m4-exercise-files`
* :computer: [exercise 01](./TDD_ex01/readme.md): Unit testing with JUnit and Hamcrest
  * :computer: [solution](./TDD_ex01_solution/) (this link will be enabled when the solution is released)

Solutions to exercises will be posted under this folder on GitHub as projects with the name `${ExerciseName}_solution`.
  
## Week 2. Behaviour-driven development 

In this week, we are going to buid on what we learned about **test driven development (TDD)** for introducing **behaviour driven development (BDD)** using Spock.

### What to focus on?
* Revision of Spring MVC and TDD using quizzes
* Behaviour-driven development: RED/GREEN/REFACTOR
* Spock
  * given/when/then/expect/where
  * Data-driven testing and method unrolling
  * Reporting failures
* Integration testing
  * MockMvc objects
  * Spring MVC Testing Framework
  

### Exercises (formative coursework)
* :computer: [Exercise 02](./TDD_ex02/readme.md): Introduction to Spock 
  * :computer: [solution](./TDD_ex02_solution/) (this link will be enabled when the solution is released)
* :computer: [Exercise 03](./TDD_ex03/readme.md): Using Spock in a Spring MVC project
  * :computer: [solution](./TDD_ex03_solution/) (this link will be enabled when the solution is released) 

Solutions to exercises will be posted under this folder on GitHub as projects with the name `${ExerciseName}_solution`.

## Additional resources (for reference)

These are pointers to official documentation in case you need to deepen your knowledge when implementing the mini project:
* [Spock Framework](http://spockframework.org/spock/docs/1.1/)




