2020/ICT/30 -> 
 My contribution 
    1)index.js ->index is entrypoint of an application.
    2)seed.js->seed.js used for initiate the admin usernames and passwords.
    3).env->.env used to security purpose and store url of database and store secret keys.
    4)middlewears ->   
         adminmiddlewear.js,
         authmiddleweare.js,
         appliedadminmiddleware.js,
         boysadminmiddleware.js,
         bsadminmiddleware.js
             above middleware.js used for Authorization Header Check and JWT Verification.
             When we using middleware.js file to verify token we have to insert this to function like this
             example => router.get("/example",middleware.js, async(req,res)=>{}).
    5)routes -
         authroute.js
             functions -> (used post methods for below functions)
                 authroute has register,userlogin,
                 mainadmin login,
                 appliedcanteen admin login,
                 bs canteen admin login,
                 boyshostelcanteen admin login.
    6)models -
         adminmodel.js
         usermodel.js
             we used models in nodejs improve Reusability,Database Interactions,Data Abstraction and Encapsulation(provide clear structure).
    *modules->express,nodemon,dotenv,cors,jsonwebtoken,bcrypt,mongoose,morgon          


2020/ict/52
userroute functions:
  GET user (find user,hide password,response for the get user)
  Update User(validate,update,save the user details)
  Reset Password
  Delete User
  diplay canteens
  display Foods by Applied Canteen
  display Foods by Bs Canteen
  display Foods by boyshostelcanteen
  display Foods for Applied Canteen Admin
  display Foods for Bs Canteen admin
  display Foods by boyshostelcanteen

2020/ICT/18
functions:
GET admin
Find admin
Delete canteen
display applied canteen orders
display Bs canteen orders
display BoysHostalcanteen orders
Display Payments

2020/ICT/95
My contributions:
 Food,order and payment models:
 Integrated comprehensive models to handle food items, orders and payment processing.
  foodsmodel.js -> Defines the schema and model for food items in this application, using mongoose and ODM library for MongoDB and Mode.js
                   This file handles the structure validation of food data and provide a way to interact with foods
  ordermodel.js -> Defines the structure of order docs specifying data types and validation rules
  paymentmodel.js->Defines the schema and model for handling payment transactions in our application

  mongodb.js ->Manages the configuration and connection to the mongoDB database in our application

2020/ICT/64
My Contributions: Canteen Route and Model
canteenmodel.js -> This file defines the schema and model for storing canteen information in the database using Mongoose.
Schema-> The canteensceema includes fields for Canteenname, openclosetime, and description.
Model Export -> The schema is compiled into a Mongoose model named canteen and exported for use in other parts of the application.
canteenroute.js -> This file sets up the routing for canteen-related operations using Express.

2020/ICT/107
  My Contributions: 
  Routes and Middleware Integration for Food, Order, and Payment Management
    I set up routes and middleware to manage the application's food items, orders, and payments. Here's a summary of what I did:
    1. Express Setup and Middleware:
       - Configured the Express app with middleware for user authentication and authorization.
    2. Add Food to Canteens:
       - Created routes to add food items to different canteens (applied, BS, and boys' hostel) with checks for necessary details like food name, price, available time, and image URL.
    3. Delete Food by ID:
       - Made a route to delete food items by their ID, ensuring only authorized users can do this.
    4. Update Food Details:
       - Added a route to update food details, making sure the food item exists and all necessary fields are provided.
    5. Place and Manage Orders:
       - Developed routes to place new orders, update existing ones, and delete orders. This includes validating order details and calculating the total payment amount.
    6. Payment Processing:
       - Implemented a route to handle payments, collect payment details, and update the payment status.
    7. Display Payment Information:
       - Added a route to show payment information to users, ensuring the payment record exists before displaying it.
canteenmodel ->Mongoose model for canteen data.

canteenmodel.js: Provides a structured schema for canteen data, ensuring consistency and validation in the database.

canteenroute.js: Implements the necessary routes for creating canteen entries, including middleware integration for security and authorization checks.
 
