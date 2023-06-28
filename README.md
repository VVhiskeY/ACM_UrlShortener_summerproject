### ACM_UrlShortener_summerproject
URL shortening tools convert long, complex URLs into shorter, more concise ones. They are beneficial for sharing links on social media due to character limits. Shortened URLs are easier to read, visually appealing, and encourage click-through rates. Additionally, these tools often provide analytics to track link clicks, allowing you to measure the success of your marketing campaigns. 

## Installation

Install node.js on your device for the backend part of the project.

Install express , mongoose , ejs , shortid , dependencies :

npm i express mongoose ejs shortid

Install nodemon as a dev dependency :

npm i --save-dev nodemon

## Getting Started

To start the server we can go to package file and add script : "devStart": "nodemon server.js"

then give below command to start the server :

npm run devStart

## Internal Working

When we start the server the frontend sends the requests to backend to fetch the data then the backend sends data to frontend which we can see on the main webpage . When we input some URL to be shortened and the note corresponding to it than a post request is send to backend to short the URL and add original URL , Note , shortened URL and the number of clicks to the database and display it on the main webpage :


Every time a user clicks on the shortened URL the number of clicks get incremented by 1 for that URL and on refreshing the page we can see the changes . For the database functioning a Schema object was created containing the structure to store the above described data and then a model was created based on that Schema object using mongoose.model(). The model will allow us to perform database operations on corresponding collection . For search functionality when we input some text in the search bar the search request is processed and we get the filtered data from the database by the help of find() function :


The search feature is applied to full url , note and the shortened Url also for the user convenience.

## Lessons Learned

Get to know about Basic HTML, Javascript,EJS and Node.js .
setting up MongoDB database , properties of host.
Working with Bootstrap and its basic commands to make good UI for website


# Search functionality :

By learning to work with $regex operator of MongoDb and the find function .



## References & Resources used

HTML tutorial :
https://www.youtube.com/watch?v=pQN-pnXPaVg

CSS tutorial :
https://www.youtube.com/watch?v=yfoY53QXEnI

JavaScript tutorial :
https://www.youtube.com/watch?v=PkZNo7MFNFg

Node.js and Express.js tutorial :
https://youtu.be/Oe421EPjeBE

EJS tutorial :
https://www.youtube.com/watch?v=VM-2xSaDxJc

Mongoose tutorial :
https://www.youtube.com/watch?v=DZBGEVgL2eE

MongoDB tutorial :
