# MMO Chess

### MMO chess is a multiplayer 3 minutes (per player) chess game made using Socket.IO

* Mongo DB
* Node JS

#### Run the application

Run Mongo db using :

```
$> mongod
```

or `sudo mongod` depending on your OS =)


Download the node packages and dependecies :
```
$> npm install
```

Run the server:
```
$> node .
```

By this the game should be running on `http://localhost:3000`

## MMO Chess Project structure:

* Client  
    * Socket.io(Socket.IO enables real-time bidirectional event-based communication)
    * HTML5, CSS3, JavaScript, jquery and the awesome bootstrap and font awesome to add the icons


* Server :
    * Handlebars.js for rendering HTML templates
    * Node JS web server
    * Mongo DB as database
    * Express JS as web framework
    * Passport JS for authentication
    * Socket.io


## Features of this Project :

* Multiplayer game that consists of two players connect trough sockets using socket.io
* Used passport.js for User authentication to signup and login
* REST APIs `/api`


# Functionality :

1. Admin enables the tournament date and time.
2. Players after entering a room(can contain 20 players), join a random table with other player.
3. when the second player joines the game, server connects the two player's sockets to the same socket.io room and the game starts once they have connected
4. The timer starts for both the players for 3 minutes
5. when the game ends after the time lapse for at least one player, both players are disconnected and scores updated

## RESTFUL API

## User

* Send a GET request to

`` /api/user/:name ``

Example:

``
/api/user/khaled
``

```
{
    "id": "123",
    "name": "khaled",
    "email": "khaled.dawodieh@gmail.com",
    "lastConnection": "now :p "
}
```
