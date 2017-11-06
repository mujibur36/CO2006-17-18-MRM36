<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Primer/3.0.1/css/primer.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/octicons/3.5.0/octicons.min.css">

# IDE and Tooling

The tools that need to be installed in your machine in order to do the exercises for CO2006 17-18 are:
* Java 8
* The Spring Tool Suite (STS) 3.9.0
* Groovy 
* Gradle Buildship

Find below:
* [An installation guide of the tools required.](#installation-guide)
* A [tutorial on Eclipse](#exploring-eclipse-sts), the IDE (Integrated Development Environment) behind the Spring Tool Suite, exploring the different parts of the environment. This tutorial will show you how to organize your Java projects in Eclipse and how to run/debug them.
* [Instructions to set up your workspace for CO2006 17-18.](#setting-up-your-github-repository)

## Installation guide

A screencast describing how to install the STS, Groovy and Gradle is available :movie_camera: [here](https://leicester.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=01817d03-6f37-49d9-be77-dd079906e407).

Further considerations on the tools that we are going to use in CO2006 are described below.

### Java 8

* Download Java 8 from [Oracle's website](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html).
* Install it.

### Spring Tool Suite (STS) 

* Download the Spring Tool Suite (STS) 3.9.0 available from [the Spring website](https://spring.io/tools).
* Unzip and move to:
  * Mac OS: `Applications` 
    * In some cases, you may not be able to install Groovy plugins, with the error being that you don't have write permissions on the installation folder. If you drag and drop the STS file to the `Applications` folder, you may be able to install the plugins.
  * Windows: `Program Files`
    * Use 7-zip ([http://www.7-zip.org](http://www.7-zip.org)) to unzip the zipped file that you get when you download the STS.
    * Some students could not install the STS under the folder `Program Files`. If that is your case, try to install the STS in another folder, e.g. in `My Documents`. 
  * Linux: your folder of choice

### Groovy

* From within STS (launch it first).
* `Help > Dashboard` (from Spring perspective).
* `Manage > IDE extensions`.
* Select:
  * `Groovy 2.4 compiler for Groovy-Eclipse`;
  * `Groovy-Eclipse`;
  * `Groovy-integration with m2clipse` .
* Click `Install` and follow the instructions.

### Gradle

* From within STS (launch it first).
* `Help > Eclipse Marketplace`.
* Search for `Buildship Gradle Integration 2.0`.
* Install it and follow the instructions.

## Exploring Eclipse (STS) 

You need access to Pluralsight, [send me an email](mailto:ab373@le.ac.uk) if you can't access them.

* :movie_camera: [Why Eclipse?](https://app.pluralsight.com/player?course=eclipse-guided-tour-part1&author=tod-gentille&name=eclipse-guided-tour-part1-m1&clip=2&mode=live)
* :movie_camera: [The workspace - launching Eclipse](https://app.pluralsight.com/player?course=eclipse-guided-tour-part1&author=tod-gentille&name=eclipse-guided-tour-part1-m1&clip=7&mode=live)
* :movie_camera: [Eclipse workbench overview (skip c++ sections)](https://app.pluralsight.com/player?course=eclipse-guided-tour-part1&author=tod-gentille&name=eclipse-guided-tour-part1-m2&clip=0&mode=live)
* :movie_camera: [Demo: Importing Java Sample Files: importing files into your workspace](https://app.pluralsight.com/player?course=eclipse-guided-tour-part1&author=tod-gentille&name=eclipse-guided-tour-part1-m3&clip=1&mode=live)
* :movie_camera: [Package/project explorer (first three minutes)](https://app.pluralsight.com/player?course=eclipse-guided-tour-part1&author=tod-gentille&name=eclipse-guided-tour-part1-m3&clip=3&mode=live)

## Setting up your GitHub repository

We are going to use two repositories on GitHub, the main one `CO2006-17-18`, which is going to be used to release new resources, and your own private repository `CO2006-17-18-${YourGitHubUsername}`, which is going to be used to do coursework.

### Main repository CO2006-17-18

Follow these steps:
* Create an account on GitHub if you don't have one already.
* Fill in [this Google form](https://goo.gl/forms/aulECrDmKpctM0A33) and provide your GitHub username (you may need to log in with your Google credentials).
* You will be invited (via an email to your GitHub email account) to access the resources during the week starting on `2nd October 2017`.

This repository is intended to be used in **READ-ONLY MODE**. That is, do not write or modify any file or folder in your local copy of the repository. If you do it accidentally, please delete the whole local copy of the repository and clone it again. 

### Your individual repository CO2006-17-18-${YourGitHubUsername}

GitHub is used to submit assessed coursework. Please accept [this invitation](https://classroom.github.com/a/wRmC0JoX), which will create your individual private repository on GitHub, and clone it in the STS as explained :movie_camera: [in this video](https://leicester.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=cfcff53c-142c-48ee-aa7d-95acb3e57530). The video also explains how to import the exercises for sprint 1.

This repository is intended to be used in **READ-WRITE MODE**. That is, this is your private repository and you have control over its contents. This repository can be used to keep backup copies of your work and to submit your coursework.

:movie_camera: [This video](https://leicester.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=fcc8ee35-cee8-4b83-9c02-38de6bacd81b) illustrates how to transfer files from the master repository to your private repository.
