# GDP Tickets Template

- Author: Mothusi Molorane
- Date: 15-Feb-2022

This document was created to assist you create tickets for projects. Will present each epic and
possible tickets under each epic.

## Java course
- Course 1: Java - JVM, Java Language, Garbage Collector
- Course 2: Java - Java Fundamentals, String
- Course 3: Java - OOP
- Course 4 : Java - JBDC
- Course 5: Java - Generics, Collections
- Course 6: Exception Handling
- Course 7: Lambda expresions, Stream API
- Course 8: Multithreading
- Course 9: DateTime API
- Course 10: Annotations, Reflection

## Frontend [Angular, React, Vue]
- `Create a blank screen` - Create initial blank screen on angular.
  Definition of done: Have a default hello world screen display when you start the application.
- `Research UI library and create mock data` - Research and create mock data for medical plans. Definition of done research a library that can assist with rendering UI components and loaded some mock data in a typescript array / json file.
To prove that research was completed they will have to present back to the team 2 types of UI libraries describe benefits/ disadvantages and a brief description and mention which one they think will be suitable for the project.
- `Scaffold the approved medical plans design` - Render the approved initial medical plans layout page using a UI library.
  - Definition of done:
    - Page rendered according to design (try to mimic the design as best as possible)
    - Use the mock data (json file) to render the medical plans
- `Render elements dynamically from API response` - Display medical plans dynamically from the data received from the Tiger Backend
  - Definition of done:
    - Generate an angular client using an OpenAPI file. 
    - Call the Tiger backend and receive the medical plans information successfully. 
    - Display the medical plans according to the data received from tiger.
- `Design initial forms` - Design the form users need to fill in order to sign up for a specific medical plan.
   - Definition of done: 
     - Clear design that displays where buttons and fields will be located. 
     - Fields principal user 
       - idnumber 
       - name and surname 
       - salary 
       - medical plan chosen 
       - email + password
- `Scaffold initial signup page` - Definition of done: scaffold the initial user page where a user can enter their details to signup for a specific medical plan.
- `Add 'select medical plan' on all plans`
- `Create a component store for medical plans` - Research how to manage state on angular. After which you will have to create component store for medical plans. 
  - Basically update your previous task to get the data from a store. 
  - Definition of done: Medical plan date is accessed from the created store.
- `Design form to get user data` - Have a look at the table design: https://bitbucket.org/bsgafrica/backend/src/f9477771a5d0/Tiger%20Database%20Design.jpg . Then design a form to get the appropriate user data.
  - Definition of done: The form is designed with fields to get all needed user data.
- `Generate typescript models based on openapi spec` - Include openapi scripts to create frontend models for you. Update the project, creating the already created frontend model through openapi spec. 
  - Definition of done: Models are created through the openapi spec.
- `Get the list of medical plans from the service (Tiger) and display them on the frontend`
  - Definition of done:
    - Replace json data with service data 
    - The service data is rendered on the frontend
- `Filter medical plans on selection` - Implement the filter mechanism on the medical plans page.
  - Definition of done:
    - A user should only see the plans based on the selected filter 
    - A user can decide that they want to see medical plans that are above or bellow R200 as an example.
- `Sort medical plans` - The medical plans will be sorted based on the selected sort variable
  - Definition of done:
    - When the user select sort variable, medical plans should be displayed in sorted order, regardless whether is Rhino or Lion.
- `Implement the user form` - The task is to implement this design: https://bsg.atlassian.net/jira/software/projects/GB2/boards/17/roadmap?selectedIssue=GB2-159
- ``


## Tiger Back-end
If this Dart package is published to Github, add the following dependency to your pubspec.yaml

- `Create initial api implementation to return dummy response` - Return dummy response of medical plans using the OpenAPI spec.
  - Definition of done: 
    - The api end point is able to list the  dummy data when called. Write unit test to test the logic on your service implementation.
- `Design initial medical plans layout` - Use a wireframe tool to design the initial look of the medical plans page. 
  - Definition of done: design complete and approved.
- `OpenAPI spec to get all medical plans` - Create the OpenAPI spec that defines the endpoint on obtaining all medical plans.
  - Definition of done: 
  - Created the OpenAPI spec that includes a medical plan object. This should be done in the bsgafrica / backend — Bitbucket .A medical plan object fields includes:
    - Id 
    - Name 
    - Price
- `Edit api implementation to retrieve medical plans from Rhino and Lion` - Edit the initial API implementation to retrieve the medical plans from Rhino (soap) and Lion (rest)
- `Edit OpenAPI spec to include path to sign up a user for a medical plan`
  - Definition of done: 
    - Edit the existing openAPI spec to include signing up a user for a medical plan.
- `Research on migration scripts and create user table through the script`
- `Update chick-style file with our own standard`- Come up with a list of standards to add on the file. As an example  the list can include the rule to enforce all models created by the openaoi to end with DTO postfix.
  - Definition of done: 
    - You have tested the file on your local machine and created the PR.
- `Understand Hibernate to create repository object for medical plan table` - Learn how hibernate works. Implement Hibernate concepts to create repository interface for medical plan table/object.
  - Definition of done: 
    - Medical plan repository can communicate with h2 db
- `Get the medical plans from the db` - Update the initial implementation done on ticket: GB2-12: [Tiger Backend Downstream] Create initial api implementation to return dummy responseDONE to now get the data from the h2 db
  - Definition of done: 
    - Able to use postman to get all the medical plans from the db
- `Scaffold Cucumber Testing` - Cucumber is useful for acceptance testing, allows for writing tests in something like plain english and doing so in a behavioral driven way. Correlates to business user stories which need to be “accepted”.
  - Definition of done:
    - Research cucumber 
    - Get cucumber 
    - Configure cucumber 
    - Write one dummy test 
    - Make sure it runs when run as part of local maven test
- `Create medical plan tables using migration script` - Create the table using migration script.
  - Definition of done: 
    - Running the script create the table on the db and the script should be able to run on both h2 and pro db
- `Create a chick-style file` - Add a check-style file to all the projects (Tiger, Rhino, Lion).
  - Definition pf done: 
    - The fine is included in all the project, and is able to suggest on code mistake.
- `Wrap front end project in maven` - Find out how to include your angular front-end project into maven.
  - Definition of done: 
    - Angular front-end project is wrapped  into back-end project using maven.
- `Load dummy data into medical plan db` - Through migration script load dummy data into medical plan database.
  - Definition of done: 
    - The database is loaded with dummy data through the migration script.
- `Retrieve medical plan from Lion` - Find a technology you can use on your project to call Lion endpoint to retrieve medical plans and save the data on Tiger database.
  - Definition of done: 
    - Retrieve medical plans from Lion and save the plans onto tiger database.
- `Retrieve medical plans from Rhino` - Find a technology you can use on your project to call Rhino endpoint to retrieve medical plans and save the data on Tiger database.
  - Definition of done:
    - Retrieve medical plans from Rhino and save the plans onto tiger database.
- `Add authentication (JWT)` - Add an authentication mechanism to the Tiger backend. The authentication to be implemented should be JWT.
Note: The expectation is that this task will take you at lest more than a day to complete. So, please take your time, what we are are looking for is understanding not how quickly you can complete the task.
  - Definition of done:
    - Table for storing user credentials is designed and created if its not there already. And the user can be authenticated using JWT mechanism.
- `Update Tiger OpenApI spec to include database changes` - Include Benefit and MedicalPlanBenefit (bridge table) Objects
  - Include Company Object 
    - Add Description field to MedicalPlan Object 
    - migration script for the tables 
    - Add dummy data to the tables 
  - Definition of done:
    - Updated Tiger OpenAPI spec with new tables, field, and dummy data loaded.
- `Design database that includes the relationships between a user and medical plan` - We need to store our user data and medical plan data in a database. Design the database tables that includes the relationships between a user, medical plan and dependents.
Note: a principal user should be able to sign up for a medical plan they chose, and they should be able to add more than 1 dependents if they choose to do so. A dependent can be a spouse, child etc.
  - Definition of done:
    - Database includes all relevant fields to store user data.
    - Database includes the correct relationships between principal user, dependents and medical plan.
  - User field includes:
    - Id 
    - Id number 
    - Medical plan chosen. 
    - Cover start date
  - Medical plan fields:
    - id 
    - name 
    - price
  - company: whether the medical plans is from lion/rhino
- `Register user in database`
  - Definition of done: 
    - retrieve the data from the frontend and store the data in the database.
## Rhino SOAP
- `Create spec for getting all medical plans` - Create the OpenAPI spec that defines the endpoint on obtaining all medical plans.
  - Definition of done: 
    - Created the OpenAPI spec that includes a medical plan object in the bsgafrica / soap — Bitbucket
- `Research options for defining SOAP service API` 
  - Definition of done:  
    - present back the options found for SOAP service API, discuss advantages and disadvantages and team will decide which option to use. 
    - Research on xml, wsdl and XSD and how it relates to Java. 
    - Research if OpenAPI is a possible solution . 
    - Soap UI
- `Create initial api implementation to return dummy response` - Return dummy response of medical plans using the OpenAPI spec.
  - Definition of done:
    - Should have DB table for medical plans, which includes name, id and price. (research h2 database).
    - Should have associated Hibernate Entity and Repository for said table.
    - Should return all entries from DB in API response (mapped to the response type via mapper - use mapstruct)
    - Insert two dummy records for above table.
    - Unit test the service method, and write an integration test for repository method, and write cucumber test for whole method.
    - Use Postman to call the end point and receive the dummy response.
- `Create a Mapper util class` - Create a mapper util class. The class should have util methods to map objects to other objects.
  - Definition of done: 
    - The mapper util class is created with at lest one method.
- `Write unit and integration tests` - Write both unit and integration for the services created,
  - Definition of done: 
    - All negative and positive test cases are implemented and all the tests are passing.
- `Load data into the db using migration script` - Load dummy data into the db using migration script
- `Return medical plans from the database` - Edit the endpoint to return medical plans stored in the database.
- `Create migration scripts to create medical plan table` - create scripts to create medical plan tables based on the properties inside the openAPI spec Make sure to set the profiles ,Use liquibase
- `Add OAuth authentication mechanism` - Add a server side authentication on Rhino server Service. The authentication mechanism to be implemented is OAuth. Definition of done:  Tiger project can authenticate with Rhino server service, when consuming APIs.

## Lion Rest
- `Create initial api implementation to return dummy response` - Return dummy response of medical plans using the OpenAPI spec.
  - Definition of done: 
    - The api end point is able to return the  dummy data when called.
- `Create OpenAPI spec for getting all medical plans` - Create the OpenAPI spec that defines the endpoint on obtaining all medical plans.
  - Definition of done: 
    - Created the OpenAPI spec that includes a medical plan object in the bsgafrica / api — Bitbucket .A medical plan object fields includes:
      - Id
      - Name
      - Price
- `Load data into the db using migration script` - Through migration script load dummy data into medical plan database.
  - Definition of done: 
    - The database is loaded with dummy data through the migration script.
- `Create a Mapper util class` - Create a mapper util class. The class should have util methods to map objects to other objects.
  - Definition of done: 
    - The mapper util class is created with at lest one method.
- `Return medical plans from the database` - Edit the endpoint to return medical plans stored in the database.
- `Create migration scripts to create medical plan table` - create scripts to create medical plan tables based on the properties inside the openAPI spec Make sure to set the profiles, Use liquibase
- `Add OAuth authentication mechanism`
- `Add more variables on the check-style` - Update the check-styles for more variables and copy them other specs
  - Definition of done:
    - Check style script is updated with missing variables and still runs successfully.
- `Write unit and integration tests` - Write both unit and integration for the services created,
  - Definition of done:
    - All negative and positive test cases are implemented and all the tests are passing.

## Infrastructure
- `Setup terraforms script to create virtual machine` 
  - Definition of done:
  - Research terraforms and virtual machines 
  - Use terrafroms to define and create the virtual machine 
  - Configurative terraform script that can access the virtual machine. 
  - Authentication keys that give everyone in the bootcamp access to the virtual machine
- `Create ansible playbook to deploy`
- `Update terraform script to authenticate all team members` - Find out how to update terraform scripts. Request public keys from your team members and update the terraform scripts to include the keys.
  - Definition of done:
    - Terraform scripts is updated with the keys and it runs successfully.