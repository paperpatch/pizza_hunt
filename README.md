# Pizza Hunt

Pizza Hunt is a server that allows users to create their own masterpiece pizza while other users contribute value by commenting and replying to comments. Pizza Hunt uses `MongoDB` to set up the database and `Heroku` to deploy the server. This application utilizes NoSQL MongoDB.

## Table of Contents

* [Setup](#setup)
* [Usage](#usage)
* [Deployment](#deployment)
* [Contributing](#contributing)
* [License](#license)

## Setup
:floppy_disk:

The database uses the following npm:

- [Node Package Manager](https://nodejs.org/en/)
  - Run `npm install` in order to install the following npm package dependencies as specified in the `package.json`.
  - This will also help install express on your system and manage any other dependencies in your script.
- [Express](https://www.npmjs.com/package/express)
  - A minimal and flexible Node.js web application framework that provides a robust set of features to develop web and mobile applications. Facilitates the rapid development of Node based Web applications.
- [Mongoose](https://www.npmjs.com/package/mongoose)
  - Mongoose is a MongoDB object modeling tool designed to work in an asynchronous environment. Mongoose supports both promises and callbacks.

This repository uses the following server:

- [Heroku](https://heroku.com/)
  - A cloud application platform service that enables developers to build, run and operate applications entirely in the cloud.
- [MongoDB](https://www.mongodb.com/)
  - Source-available cross-platform document-oriented database program. Classified as a NoSQL database program.

<br/>

### Model Setup

- Pizza Schema
  - pizzaName
  - createdBy
  - createdAt
  - size
  - toppings: []
  - comments

<br/>

- Comment Schema
  - writtenBy
  - commentBody
  - createdAt
  - replies: [ReplySchema]

<br/>

- ReplySchema
  - replyId
  - replyBody
  - writtenBy
  - createdAt

## Usage

:computer:

Go to the [deployed](https://pizza-hunt-program.herokuapp.com/) app at Heroku

Users are able to create their own masterpiece pizza and share it on the server. Other users are able to comment on the pizza and reply on other user's comments.

## Deployment

Deployed at Heroku:

[Deployed Link](https://pizza-hunt-program.herokuapp.com/)

## Contributing

:octocat:

[paperpatch](https://github.com/paperpatch) </br>

## License

:receipt:

