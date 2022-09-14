# rap-name-api
This is a simple API that lets you get generic information about 21 Savage and Chance the Rapper. 

**Link for server:** https://rap-names-api-ld.herokuapp.com

![alt tag](https://i.imgur.com/itKqjw3.png)

## How It's Made:

**Tech used:** Node.js with Express, HTML

The API has a get method that responds to "21 Savage" and "Chance the Rapper" (not case-sensitive) when searched. If a user searches for something else, the server
will respond back with "unknown". The server is hosted and deployed through Heroku.

Side note: There is no client-side JS. The .html included is only used to display a webpage for testing purposes only.

## Lessons Learned:

This project taught me how to implement the read operation from the CRUD convention. By using app.get('/api/:yourVariableName') you set up your
server to listen to different query searches and return information. The cors node module is needed in order to allow other clients to access your API. 
Specifically to Heroku, I must pass process.env.PORT to app.listen() since Heroku will choose a port of it's own. 

Additioanlly I gained first-hand experience with express which made it easier to build my own API and kept my code base cleaner. 

