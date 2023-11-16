## nodejs-graphql
npm init -y
npm i express

## install nodemon globally
npm i nodemon

## install nodemon dev
npm i nodemon -D

## add in package.json under scripts
"dev": "nodemon server.js"

## use nodemon
npm run dev

## install graphql with express
npm install graphql express-graphql

## import graphql
const graphql = require("graphql");
const { graphqlHTTP } = require("express-graphql");

## access 
http://localhost:6969/graphql

## query -> get all users
query {
  getAllUsers {
    firstName
    lastName
    email
    password
  }
}

## mutation -> create users
mutation {
createUser(firstName: "Dale", lastName:"Lanto", email: "dalelanto.work@gmail.com", password:"password") {
    firstName
    lastName
    email
  }
}

mutation {
  
  createUser(firstName: "Jesabel", lastName:"Ducena", email: "jesabelducena@gmail.com", password:"password") {
    firstName
    lastName
    email
  }
}

