<link rel='stylesheet' href='./web/swiss.css'/>

# Sprint 1: Agile practices and build automation

In this sprint, we are going to focus on the main phases and principles behind common software development methodologies. We will analyse common software development practices from a critical point of view and we will use specific tools to manage software development. Namely, we will use Groovy and Gradle for automating software builds.

The sprint for the following two weeks is structured as follows:
* We will cover software development methodologies.
* We will learn Groovy, a scripting language used to program Gradle build scripts.
* We will learn how to program Gradle build scripts using Groovy for Java projects.

At the end of this page you will find a jargon buster on terms that may be new to you.

## The Sprint Goal (assessed coursework)

The goal for this sprint is a test on agile practices in software development, Groovy and Gradle. The syllabus to be assessed is highlighted in the description of each unit below.

Specific organization details about the test are as follows:
* :dart: **TEST**: Tuesday 17th October, CW3 Lab (out of 100, weight: 15%)
  * [Group A](https://github.com/uol-inf/CO2006-17-18/blob/master/groupA.md): 16:00-16:50
  * [Group B](https://github.com/uol-inf/CO2006-17-18/blob/master/groupB.md): 17:00-17:50
* :computer: A sample test is available [here](https://blackboard.le.ac.uk/webapps/assessment/take/launchAssessment.jsp?course_id=_1807_1&content_id=_1425217_1)
* :notebook: [Revision session handouts](./sprint1_revision.pdf)

## Week 1. Agile practices

* :movie_camera: [Lecture 02](https://leicester.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=5802c9d7-b09f-4426-89c3-70be77c159bd)
  * :notebook: [Lecture 02 handouts](./L02_handouts.pdf)

### Software develoment methodologies

In this unit, we are going to become familiar with the main phases of software development and the principles behind the main software development methodologies. 

#### What to focus on?

In the videos below, we are going to focus on:
* waterfall methodology:
  * software project lifecycle and main phases of software development
  * pros/cons
  * where it is recommended/discouraged to use it
* V-model:
  * how testing complements each phase of the waterfall model
  * pros/cons
  * where it is recommended/discouraged to use it
* agile methodologies:
  * what are the core values?
  * what are the main principles of the agile manifesto?
  * what are the common misconceptions and mistakes (risks) to be avoided?
  * pros/cons
  * where it is recommended/discouraged to use it

#### Pluralsight resources
* :movie_camera: [Waterfall Fundamentals and Its Problems](https://app.pluralsight.com/player?course=agile-fundamentals&author=stephen-haunts&name=agile-fundamentals-m2&clip=0&mode=live)
* :movie_camera: [What is agile all about?](https://app.pluralsight.com/player?course=agile-fundamentals&author=stephen-haunts&name=agile-fundamentals-m3&clip=0&mode=live)
* :movie_camera: [Common agile misconceptions](https://app.pluralsight.com/player?course=agile-fundamentals&author=stephen-haunts&name=agile-fundamentals-m4&clip=0&mode=live)
* :movie_camera: [Advantages and disadvantages](https://app.pluralsight.com/player?course=agile-fundamentals&author=stephen-haunts&name=agile-fundamentals-m5&clip=0&mode=live)
* :black_nib: [Learning check](https://app.pluralsight.com/library/courses/agile-fundamentals/learning-check)

### Groovy

In this unit, we are going to cover the basics of Groovy's syntax so as to be able to read and write Gradle build scripts. 

#### What to focus on?

* What is Groovy? What are its main features?
* How to write and run Groovy scripts?
* Working with collections and ranges
* Writing and using functions
* Writing and using closures
* Differences between functions and closures
* Dynamic capabilities

#### Pluralsight resources

* :movie_camera:  [Introduction](https://app.pluralsight.com/player?course=groovy-fundamentals&author=jeremy-jarrell&name=groovy-fundamentals-m1&clip=0&mode=live): General introduction and motivation for scripting languages.
* :movie_camera: [Basic syntax](https://app.pluralsight.com/player?course=groovy-fundamentals&author=jeremy-jarrell&name=groovy-fundamentals-m2&clip=0&mode=live): You should get familiar with the syntax in order to be able to read and customize Gradle build scripts.
* :computer: Check the [examples used in Pluralsight](https://app.pluralsight.com/library/courses/groovy-fundamentals/exercise-files).

#### Exercises (formative coursework)

* :black_nib: [Learning check](https://app.pluralsight.com/library/courses/groovy-fundamentals/learning-check)

For doing formative and assessed coursework, set up your own private [as explained in the tooling section](https://github.com/uol-inf/CO2006-17-18/blob/master/tooling.md). Once your private repository is set up, do the following exercise:

* :computer: [Exercises with Groovy](./Groovy_exercises/readme.md)
  * :computer: [solution](./Groovy_exercises_solution/) (this link will be enabled when the solution is released)

Solutions to exercises will be posted under this folder on GitHub as projects with the name `${ExerciseName}_solution`.

## Week 2. Automating builds with Gradle


In this unit, we are going to focus on automating software builds with Gradle based on what we have learnt about software development methodologies and Groovy. 

* :movie_camera: [Lecture 03](https://leicester.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=9885d588-cd0a-45b8-b11b-6efa0ddba957)
  * :notebook: [Lecture 03 handouts](./L03_handouts.pdf)

### What to focus on?

In particular, when going through Pluralsight resources, we are going to focus on:
* What is Gradle?
  * What is the Gradle wrapper?
* What is a Gradle task?
  * Writing and running tasks.
  * Specifying task dependencies.
* What is a typed task?
  * Using the copy task.
* How to use Gradle to build a Java project?
  * What is a Gradle plugin?
  * Tasks offered by the Java plugin
  * What is the Gradle daemon
  * **Multi-project builds are not assessed**
* How does Gradle handle library dependencies?
  * What is a repository?
  * Using repositories of libraries
* How do you run Java tests from Gradle?

### Pluralsight resources

* :movie_camera: [Introduction](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m1&clip=0&mode=live)
* :movie_camera: [Basic Gradle Tasks](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m2&clip=0&mode=live): Explains what you can do in a Gradle build file.
* :movie_camera: [Task dependencies](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m3&clip=0&mode=live): Explains how to order tasks.
* :movie_camera: [Typed tasks](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m4&clip=0&mode=live)
* :movie_camera: [Building a Java project](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m5&clip=0&mode=live): Explains how to build a Java project.
* :movie_camera: [Dependencies](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m6&clip=0&mode=live): Explains how to import depedencies (jars, other libraries, etc.) from repositories.
* :movie_camera: [Testing](https://app.pluralsight.com/player?course=gradle-fundamentals&author=kevin-jones&name=gradle-fundamentals-m7&clip=0&mode=live): Explains how to run tests. We will see how to write tests in the following sprint.
* :black_nib: [Learning check](https://app.pluralsight.com/library/courses/gradle-fundamentals/learning-check)
* :computer: Check the [examples used in Pluralsight](https://app.pluralsight.com/library/courses/gradle-fundamentals/exercise-files).

### Exercises (formative coursework)

* :computer: [Exercise 1](./Gradle_ex01/readme.md): Gradle tasks and dependencies
  * :computer: [solution](./Gradle_ex01_solution/) (this link will be enabled when the solution is released)
* :computer: [Exercise 2](./Gradle_ex02/readme.md): Java builds and Java libraries
  * :computer: [solution](./Gradle_ex02_solution/) (this link will be enabled when the solution is released)

Solutions to exercises will be posted under this folder on GitHub as projects with the name `${ExerciseName}_solution`.

## Jargon buster <a name="jargon"></a>

| term  | definition | source |
|-------|------------|--------|
| software development methodology | A methodology specifies the process to be executed, usually as a set of related activities, tasks and/or techniques, together with the work products that must be manipulated (created, used or changed) at each moment and by whom, possibly including models, documents and other inputs and outputs. In turn, specifying the models that must be dealt with implies defining the basic building blocks that should be used to construct. |  [wikipedia](https://en.wikipedia.org/wiki/Software_development_process) |
| sprint | A sprint (or iteration) is the basic unit of development in Scrum. The Sprint is a timeboxed effort; that is, it is restricted to a specific duration. The duration is fixed in advance for each Sprint and is normally between one week and one month, with two weeks being the most common. | [wikipedia](https://en.wikipedia.org/wiki/Scrum_&#40;software_development&#41;#Workflow) |
| sprint backlog | The sprint backlog is a list of tasks to be completed during the sprint. | [mountaingoatsoftware](https://www.mountaingoatsoftware.com/agile/scrum/sprint-backlog) |
| software build | Process of automating the creation of a software build and the associated processes including: compiling computer source code into binary code, packaging binary code, and running automated tests. | [wikipedia](https://en.wikipedia.org/wiki/Build_automation) |
