![Engage Spot Notion](https://user-images.githubusercontent.com/64391274/230778611-64589571-eaaa-4677-b115-7626978dd856.png)

# Engagespot API

This is a Node.js backend application that uses the Engagespot API to send notifications to users. The app exposes two endpoints: /adduser and /sentmail. The /adduser endpoint creates or updates a user in Engagespot, while the /sentmail endpoint sends a notification to a user's email address.
 
## Prerequisites

1.  Node.js 10 or higher
2.  Engagespot API key and API secret

## Getting Started

Clone the repository:

git clone 
### `https://github.com/swethatheresa/engagespot`


To install necessary packages
### `npm install` 

In the project directory, you can run:
### `nodemon index.js`

Runs the app in the development mode.\
Open [http://localhost5000](http://localhost:5000) to view it in your browser.

The page will reload when you make changes.\
You may also see any errors in the console.

## Usage

To add a user, send a POST request to /adduser with the user's email and phone number in the request body:



### POST /adduser


{


  "email": "john@example.com",
  
  
  "phoneNumber": "123-456-7890"
  
  
}



To send a notification to a user's email address, send a POST request to /sentmail with the user's email address in the request body:



### POST /sentmail


{


  "email": "john@example.com"
  
  
}


