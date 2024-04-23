🚧 **_The project structure will look like this:_**

# **TECHNICAL TEST FOR VPR**

## Introduction 📖
Automation developed to meet the technical challenge for VPR.
The automation was performed for the [Salesforce](https://login.salesforce.com/) page.

`test_salesforce` where the automation is hosted.

## Prerequisites 📋
- Java version 17 and JDK
- IntelliJ IDEA or Eclipse IDE
- Maven
- Cucumber

## Installation 🛠️🔩
- Unzip the compressed file or clone the repository:
- Import the project from Eclipse or IntelliJ IDE.
- Install and configure JDK - Java (environment variables set).
- Install and configure Maven.
- Install Cucumber plugin for Java in the IDE.

## Running the Project 🚧⚒️
- Enter the package test_salesforce \ src \ test \ java \ accountsalesforce \ runners.
- You will find 3 Runners. One executes both scenarios and a RunnerAllFeatures depending on which one you want to execute.

## Web Browsers 🌐
The automation currently runs on the following browsers:
- Google Chrome Version 123 or higher.

## General Implementation Details 💻
The test scenarios are created in the feature with Gherkin language, they are connected with a method of the StepDefinitions classes with the help of @Given, @When, and @Then annotations, the methods of the step definition are connected with Task type classes for the Given and the When, where actions are performed bringing elements from the user interface, but for the Then it communicates with Questions type classes to make validations.

   ```bash
   📦NameProject(test_salesforce)
   ┣ 📂src
   ┃ ┣ 📂main
   ┃ ┃ ┣ 📂java
   ┃ ┃ ┃ ┗ 📦[package](test.accountsalesforce)
   ┃ ┃ ┃   ┣ 📂exceptions (Classes that catch custom exceptions when automation fails and does not find an expected field.)
   ┃ ┃ ┃   ┣ 📂questions (Classes that build data models)
   ┃ ┃ ┃   ┣ 📂tasks (Classes that perform high-level actions, such as entering data into a form, etc.)
   ┃ ┃ ┃   ┣ 📂userinterfaces (Classes where the user interface elements are mapped, i.e., the web elements.)
   ┃ ┃ ┃   ┗ 📂utils (Classes that contain common functionalities.)
   ┃ ┃ ┗ 📂resources
   ┃ ┗ 📂test
   ┃ ┃ ┣ 📂java
   ┃ ┃ ┃ ┣ 📦[package](test.accountsalesforce)
   ┃ ┃ ┃ ┣ 📂runners (Classes to execute the automation with the scenarios indicated in the feature.)
   ┃ ┃ ┃ ┗ 📂stepdefinitions (Classes where the steps of the scenarios to be executed in the automation are defined.)
   ┃ ┃ ┗ 📂resources
   ┃ ┃   ┗ 📂features (Where the files with .feature extension are stored, where user stories are written.)
   ┣ 📂target
   ┣ 📜.gitignore
   ┣ 📜pom.xml
   ┣ 📜README.md
   ┗ 📜serenity.properties
 
```

## Built With 👨🏻‍💻
The automation was developed using:
- Java - Programming language.
- BDD - Development strategy.
- Screenplay - Design pattern.
- MAVEN - Dependency management.
- Selenium Web Driver - Tool for automating actions in web browsers.
- Cucumber - Framework for automating BDD tests.
- Serenity BDD - Open source library for report generation.
- Gherkin - Business Readable DSL (Domain Specific Language readable by business)

## Author ✒️👨🏻‍
**©️ Cristian Guerra Gómez** - *Project Creation.* - [criguex@gmail.com](#criguex)