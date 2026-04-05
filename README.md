# library-managment-system

This is a Library management API Backend for the management of users and the books .

# Routers and the Endpoints    

## /users
GET : Get all the list of users in the system
POST : Create or register new user

## /users/{id}
GET : Get a user by their id
PUT : Updating a user by their id
DELETE : Deleting a user by their id(check if the user still has an issued book) && {is there any fine/penalty to be collected}

## /users/subscription-details/{id}
GET : Get a user subscription details by their ID
    >> Date of subscription
    >> valid till ?
    >> Fine if any ?
    
## /books
GET: Get all the books in the system
POST: Add a new book to the system

## /books/{id}
GET:Get a book by their ID
PUT: Update a book's author name / book name by its ID
DELETE : Delete a book by its ID

## /books/issued(API)
GET : Get all the issued books

## /books/issued/withfine
GET : GEt all issued books with their fine amount

## Subscription Types
  
    >> Basic (3 months)
    >> Standard (6 months)
    >> Premium (12 months)

>  > If a user missed the renewal date,  then user should be collected with $100
>  > If a user misses his subscription , then user is expected to pay $100
>  > If a user misses both renewal and subscription , then the collected amount should be $200

## Commands:
npm init
npm i express
npm i nodemon --save-dev
npm run dev

to restore node modules or package-lock.json 
 |
 v 
npm 