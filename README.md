### ACM_UrlShortener_summerproject
URL shortening tools convert long, complex URLs into shorter, more concise ones. They are beneficial for sharing links on social media due to character limits. Shortened URLs are easier to read, visually appealing, and encourage click-through rates. Additionally, these tools often provide analytics to track link clicks, allowing you to measure the success of your marketing campaigns. 

## Prerequisites
before starting install latest versions of Node.js,Mongoose,express,

some large files are here- https://drive.google.com/drive/folders/1Ie1Al1h4kgGH8RGL5LsEcr8ETTK23nEg?usp=share_link

## Installation the dependecies

for the run the command in terminal => npm i express mongoose ejs shortid

and for nodemon  => npm i --save-dev nodemon

## Getting Started
for creating a server , add a script : "devStart": "nodemon.js" in the package file.

save this file and in terminal give command - npm run devStart

## Internal Working

After starting the server , work on back end starts using HTML main outline of file , using bootstrap overall UI ,like fonts,spacing,and colurs are defined 
When we input some URL to be shortened and the note corresponding to it than a post request is send to backend to short the URL using shortid functionality and add original URL , Note , shortened URL and the number of clicks to the database and display it on the main webpage.The number of clicks on one URL are also displayed on homepage and on refreshing the page we can see the changes.
MonogDB database is setup and linked, To enable database functionality, we created a Schema object to define the structure of the data we want to store. Using mongoose.model(), we then created a model based on that Schema object. This model allows us to perform various database operations on the corresponding collection. For implementing search functionality, when we enter text in the search bar, the search request is processed, and we use the find() function to retrieve filtered data from the database. The find() function helps us fetch the relevant data based on the search criteria provided.


The search feature is applied to fullurl , note and the shortUrl also for the user convenience.

## Lessons Learned

Get to know about Basic HTML, Javascript,EJS and Node.js .
setting up MongoDB database , properties of host.
Working with Bootstrap and its basic commands to make good UI for website
Search functionality :
By learning to work with $regex operator of MongoDb and the find function .



## References & Resources used

HTML tutorial :
https://www.youtube.com/watch?v=pQN-pnXPaVg

CSS tutorial :
https://www.youtube.com/watch?v=yfoY53QXEnI


Mongoose tutorial :
https://www.youtube.com/watch?v=DZBGEVgL2eE
