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
             functions -> 
                 authroute has register,userlogin,
                 mainadmin login,
                 appliedcanteen admin login,
                 bs canteen admin login,
                 boyshostelcanteen admin login.
    6)models -
         adminmodel.js
         usermodel.js
             we used models in nodejs improve Reusability,Database Interactions,Data Abstraction and Encapsulation(provide clear structure).


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
