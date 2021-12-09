# Mern-stack-app-Building

# Project Setup

# Frontend- Client

```
1. npx-create-react-app client




```

- default port -3000
 - use -> npm start to run the application

# Navbar

- Used bootstrap cdn -4.5 
- Used Nav component of bootstrap 







# Backend - Server 

- Node.js Environment

```
1. npm init -y 
2. npm i express --> for backend
3. npm i nodemon---> start server automatically------> use nodemon server to run the backend locally
4. npm i mongoose



```

## Entry point for the application 

- Create Express Server
- 
### Required express 

```
//=============================
//      Dependencies
//=============================
const express = require("express");

```
```
//=============================
//  Environment Variable
//=============================
const app = express();

const PORT = process.env.PORT || 5000;
```


# Database

- Connect using mongoose to the nodejs

```
const mongoose = require("mongoose");

var mongoURL = process.env.MONGOLAB_URI;

mongoose.connect(mongoURL, {useNewUrlParser: true, useUnifiedTopology: true});
# url and safety parameters

var connection = mongoose.connection

connection.on('error', ()=>{
    console.log('Mongo DB connection failed');
})

connection.on('connected', ()=>{
    console.log('Mongo DB connection worked');
})


module.exports = mongoose


```

``
use dotenv file  to protect data 

``
