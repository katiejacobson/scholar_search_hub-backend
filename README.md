# Final Project: Scholar Search Hub BackEnd

In the deployed website, information is not being returned from the Core API due to CORs policy so a server-side proxy will be built next to deal with the CORS headers.

To Be Built in Stage 2: An api that can fetch data from a local server and a db.json file will be added. Items can be added and deleted from the database.

To Be Built in Stage 3: A currentUser context will be added so that once authorization has occurred, users can access items that they have added. An api that can fetch data from a local server that is running an Express server that was created by me will been added. Users will be able to register, sign-in, as well as add, save, and delete articles from their profile.

**Description of Techniques**
Stage 2: Express.js was the framework that was utilized to create the server. A modular approach was used for routes and controllers while mongoDB and mongoose were used to create the database. A temporary authorization solution was created with authorization middleware, which allowed a user object to be added to each request. This will allow owners of cards and unique likes to be recorded.

Stage 3: Authentication and authorization steps were added so that the user schma now includes an email and password, which was hashed using cryptjs. A JSON web token was created upon login with an expiration date and authentication allows users to change their name and avatar as well as delete their own cards.

Centralized error handling was added by defining constructors for errors. Joi, celebrate, and validator packages were used to define validation functions. The winston package was used to implement request and error loggers.

## Running the Project

`npm run start` — to launch the server

`npm run dev` — to launch the server with the hot reload feature

### Testing

**Domain Name**

**Github Pages URL**
https://katiejacobson.github.io/scholar_search_hub/

**To Improve**

**Remember**
