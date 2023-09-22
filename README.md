# Spring Boot Demo Project

This is a simple Spring Boot project demonstrating how to set up a Spring Boot application, run it locally, and deploy it to an AWS EC2 instance.

## Local Setup

### Prerequisites

Before getting started, make sure you have the following installed on your local machine:

- Java 8 or 11
- Maven
- Git
- Eclipse (or any preferred Java IDE)

### Steps

1. Go to [Spring Initializr](https://start.spring.io/).

2. Choose the following configuration:

   - Project: Maven
   - Spring Boot: 2.7.3
   - Group name: com.star.agile.assignment
   - Name: springboot-demo
   - Artifact: springboot-demo
   - Packaging: Jar
   - Java: 8 or 11

3. In the dependency section, select the following dependencies:

   - Spring Web
   - Spring Data JPA

4. Click on "Explore" to verify that the `pom.xml` includes all the selected dependencies.

5. Click "Download" to download the Spring Boot Project Template (`springboot-demo.jar`).

6. Import the downloaded project into Eclipse.

7. Add the file `index.html` with some HTML code in the `static` folder under the `resources` of the project.

8. Run the Application and verify that the Tomcat server has started and is running on port 8080.

9. Verify the application by accessing the `index.html` page in your browser (http://localhost:8080).

## Deploying to AWS EC2

### Prerequisites

Before deploying to AWS EC2, make sure you have the following set up:

- An AWS account
- An EC2 instance running Ubuntu
- Git installed on your EC2 instance

### Steps

1. Install Git on your AWS Ubuntu instance.

2. Create a directory with the name "My Project" on your EC2 instance.

3. Initialize the "My Project" directory as an empty Git repository.

   ```bash
   cd /path/to/My Project
   git init
   
4. Place your Eclipse project into this Git Repository.

5. Create a .gitignore file and configure it to exclude the following files:
   *.class
   .settings
   .project

6. Add the source code to the staging area and commit it to the local Git repository.

     ```bash
    git add .
    git commit -m "Initial commit"

7. Create a Remote repository on GitHub.

8. Push the source code from the local repository to the Remote Repository.

   git remote add origin <GitHub repository URL>
   git branch -M main
   git push -u origin main

   Now your Spring Boot project is deployed on AWS EC2 and accessible through your GitHub repository.
      
