# T3A2 - Full Stack App

### By Dieter Schmid, Wenxuan Pan, Alicia Han

[Deployed Front End App](https://student-yearbook.vercel.app/)

[Deployed Back End App](https://student-year-book.onrender.com/)

[Front End Repo](https://github.com/wenxuan-pan/Full_Stack_App_T3A2-B-Frontend)

[Back End Repo](https://github.com/Dieter1978/Full_Stack_App_T3A2-B)

[Presentation](./ppt/presentation.pdf)

[Trello Board](https://trello.com/b/YU3ggBxC/school-yearbook-app)

## Table of Contents

1. [Description of website](#description-of-your-website)
2. [Dataflow Diagram](#dataflow-diagram)
3. [Application Architecture Diagram](#application-architecture-diagram)
4. [User Stories](#user-stories)
5. [Wireframes](#wireframes)
6. [Libraries Used](#libraries-used)
7. [Using the App](#using-the-app)
8. [Trello Screenshots](#trello-screenshots)

## Description of your website

A digital School Yearbook that makes a record of all student in attendance at the particular year levels of the school.

### Purpose

To display a photo, contact information and the final year thoughts of students graduating the school. This becomes a permanent online record of all graduates of the school and it can be referred to by all stakeholders of the app.

### Functionality/Features

- The app will provide admin and students accounts with a login.
- admin can add students to the app
- The student can update their details in the app.
- The Admin can upload photos and display them for all students.
- The student can fill out a questionnaire regarding their final thoughts.
- The student can provide contact details.
- Admin can invite via email students to the app

### Target Audience

This application is targetted at all school stakeholders this includes students of the graduating year level but also other students at the schools. It also includes allumi and parents of students at the school. Lastly it includes teachers and staff.

### Tech Stack

The application will utilise a MongoDB connected to a express.js server built on node.js. The front end of the application will use react.js html and css. The server and front end will be deployed to cloud services.

## Dataflow Diagram

![Dataflow Diagram](./docs/Dataflow%20Diagram.png)

## Application Architecture Diagram

![Application Architecture Diagram](./docs/Application%20Architecture%20Diagram.png)

## User Stories

User stories were split into three categories:

1. All users (students and admin)
2. Admin only
3. Students only

Throughout the planning process, we found that we needed to add and modify ideas in order for the application to work better. Hence, user stories from the beginning of the planning phase were updated to reflect these changes. We have included both sets of user stories in this documentation:

### Initial User Stories

All users:

1. As a user, I would like to be able to add a student profile into different classes/cohorts and year levels, so that student data is organised into the correct categories.
2. As a user, I would like to be able to login and view a list of students in each class and year level/cohort at my school.
3. As a user, I would like to be able to click into individual students and see their relevant information, so that I can stay in touch with classmates and connect with acquaintances.
4. As a user, I would like to have a navigation bar so that I can easily access different parts of the website.

Admin only:

1. As an admin, I want to be able to remove any profile from the database to ensure data integrity.

Students only:

1. As a student, I would like to be able to update my information, so that others can get in touch with me via my current contact details if needed, however I would like to ensure that only admin and myself can manipulate my account, for better security.
2. As a student, I want to be able to delete any information on my account, or my entire profile, from the database so that I have control over my information.

### Revised User Stories to Reflect Updated Features

All users:

1. As a user, I would like to be able to login and view a list of classes in my school, and the students in each class.
2. As a user, I would like to be able to click into individual students and see their relevant information, so that I can stay in touch with my classmates and connect with acquaintances.
3. As a user, I would like to have a navigation bar so that I can easily navigate around the application.

Admin only:

1. As an admin, I would like to see a list of all yearbooks and classes at my school, and be able to modify or delete them as appropriate, in case of error or duplication.
2. As an admin, I would like to be able to input a class of students along with their email and photos, and modify and delete student data as needed in case of error or duplication.
3. As an admin, I would like to be able to have a unique code to give to students, so they can utilise it to sign up and create their own accounts linked to the student database, this will ensure that only students who are actually in the class will be able to register to that class.

Students only:

1. As a student, I would like to have a unique code from my school admin, to be able to register as an account that is linked to a yearbook in the database.
2. As a student, I would like to be able to add, modify and delete any of my data from my account, and ensure that only the admin or myself can manipulate my account, for better security.

## Wireframes

[View in Figma](https://www.figma.com/file/wEaYAPuL9deFJ3dAndN1Fq/Yearbook-wireframes?type=design&node-id=130-2&mode=design&t=GhTV1T7VudPXjCez-0)

Mobile:

![Wireframe - Mobile](./docs/Yearbook%20wireframes%20-%20mobile.png)

Tablet:

![Wireframe - Tablet](./docs/Yearbook%20wireframes%20-%20tablet.png)

Desktop:

![Wireframe - Desktop](./docs/Yearbook%20wireframes%20-%20desktop.png)

## Libraries Used

* *express:*

* *react:*

* *bcrypt:*

* *cors:*

* *dotenv:*

* *jsonwebtoken:*

* *mongoose:*

* *nodemon:*

* *vite:*

* *vitest:*

* *react-bootstrap:*

* *toastify:*

* *jsdom:*

* *react-testing-library:*

* *react-router-dom:*

* *jest:*

* *supertest:*

## Using the App

The app has been set up with one admin user on the backend, this user will add year levels, schools and students. The login details are:

*Admin email*: john.smith@gmail.com

*Admin password*: testing

Please note that the backend test token inside src/backend/routes/test_token.js would need to be updated with the new admin token if the database is reseeded.

A student user has also been set up, the login details are:

*Student user email*: bill.smith@gmail.com

*Student user password*: anothertesting


### Installing the app locally

#### Frontend

Navigate to the frontend's folder. Use `npm install` to build the app. Use `npm run test-cc` to generate vitest coverage.

Connecting to Backend: 

The Frontend app fetches data from the deployed API by default. To change that to a local server, go to `src/utils/apiHelper.js`, and change the baseURL on line 3 (the default port for backend is 5175).

## Trello Screenshots

![Trello board screenshot - Part A](./docs/Trello%2019%20Aug.png)

![Trello - 21 Aug](./docs/Trello%2021%20Aug.png)
![Trello - 30 Aug](./docs/trello30:08:2023.png)
![Trello - 2 Sep](/docs/trello02:09:2023.png)
![Trello - 3 Sep](/docs/trello03:09:2023.png)
![Trello - subtasks](/docs/Trello%20cards.png)