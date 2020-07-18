## Introduction

This project is the backend of RentalMe, an video rental app.
The project was modified, as result of a course project path to build rest api with node, express and mongodb.
The implementation of RentalMe is in Node.js.

## 1 Setup

To run this project, you need to install the latest version of MongoDB Community Edition first.

https://docs.mongodb.com/manual/installation/

Make sure the Mongodb server is runing before continue...

### 1.2 Dependencies

From the project folder, install the dependencies:

    npm i

### 1.3 Creating Database

    node seed.js

### 2 Runing the Tests

    npm test

### Start

    npm start

The Node server will be stared on port 3900.

And you can acess the content going to:

http://localhost:3900/api/genres

You should see the list of data.

### Environment Variables (security settings)

At config/default.json, exists a property called "jwtPrivateKey". This key is used to encrypt JSON web tokens. So, for security reasons, this value should be deleted from source control.

the default value was set to make it easier for you to get up and running with this project. For a production scenario, you should delete this value and store this key as an environment variable.

On Mac:

    export rentalme_jwtPrivateKey=yourKey

On Windows:

    set rentalme_jwtPrivateKey=yourKey
