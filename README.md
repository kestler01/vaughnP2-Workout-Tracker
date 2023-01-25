# Workout Tracker

## Description

Track your gains with "My Fit", your very own customizable fitness tracker that let's you store, add, edit, or even delete your workouts. Finally! It's just like having your very own personal trainer, but on your desktop or mobile device. 

## How to run

Will fill in later

## Wire Frames

### Sign In 
![Sign In](planning/wireframes/sign-in.png)

### Sign Up 
![Sign Up](planning/wireframes/sign-up-page.png)

### User Homepage
![Homepage](planning/wireframes/home-page.png)

### Workout Planner 
![Workout Page](planning/wireframes/workout-planner-page.png)

## ERD 

### Models: User, Workout, Excercise

![ERD](planning/erd/erd.png)


## User Stories

### MVP

As a user I want to....

1. Login to account
    - Create a database to store collections. Create a user model with validation/authentication methods. If user fields pass validation, grant access to site
2. See Account info
    - On validation, user will see their current workouts (if existant), option to create workout, and option to see excercise list
3. Be able to create, edit, or delete a workout
    - A new workout model will be created for each newly created workout
    - Each workout will contain an excercise model with a many to many relationship. Each workout-plan can have many excercises and each excercise can, and will, 
        be associated with many workout-plans
    - Post newly created fields to the page and save to database for user's account
4. Be able to create, edit, or delete an excercise
    - A new excercise model will be created for each time the user uses fills in the field for 'add excercise'
        Database to store collection called 'workouts' that on submit, are stored to the collection associated with the user's account
5. Option to login or create a new account
    - Creation of a User model that stores fields for username and password. Model will use webtoken authorization and contain a 'token' field to verify
    if the token generated by their information matches that of a token stored on the database.

 
## Technologies Used
- Mongoose
- MongoDB
- Express
- Node.js
- JavaScript
- HTML
- CSS

### Ver.2

- See workout library
    - Drop down list of excersices separated by category: strength-training, cardio, etc.
- User profile picture

### Ver.3
- Api inclusion
- Description of each excercise
- Search bar the uses api to find the excercise that is typed in# Workout-Tracker
