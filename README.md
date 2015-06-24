Happy Appy Apis (Pair Projects)
===============================

Description
-----------

Happy Appy Apis (Pair Projects)

Objectives
----------

### Learning Objectives

After completing this assignment, you should…

-	Understand the importance of APIs in 2015 development
-	Understand the HTTP status codes (200, 201, 400, 401, 422, 500) and their uses
-	Understand how to serve and consume APIs in both Ruby and Rails

### Performance Objectives

After completing this assignment, you be able to effectively

-	Demonstrate ability to serve JSON via a web HTTP API endpoint
-	Demonstrate authorizing API calls via api application tokens
-	Demonstrate personalizing API calls for specific user tokens

Details
-------

### Deliverables

-	A repo containing at least:
	-	front-end Rails project (consumes API)
	-	back-end Rails project (produces API)

### Requirements

-	You'll be assigned a pair to work with.
-	Work should happen at TIY and outside as you see fit.
-	One of you will work on the front-end Rails, and another on the back-end API project.

Normal Mode
-----------

### Backend

#### Rails API Abilities

-	Create a User (email/name/secure-password) which sets a secure random key when created.
-	Create a "Sshhh" model where users can post "sshhh" (secrets)
-	Ability to Create Users
-	Ability to sign in
-	Ability to post a sshhh
-	Ability to pull the latest 20 sshhh's

### Frontend

-	The front-end web server will not store information in its database. It will get all information from the Rails API back-end server
-	Ability to create a user
-	Ability to sign in a user
-	Ability to show latest sshhh's on homepage
-	Ability to post a sshhh

Hard Mode
---------

#### Back End

-	Create an "ApiApplication" which that sets a secure random key when created.
-	Developers should be able to visit your app and create an ApiApplication and see their key.

#### Front End

-	Send along the ApiApplication token, and user token (if applicable)
-	Use remote forms to load information instead of page loads. (Login in form, Post sssh form, 'get new ssshs' button)

Nightmare Mode
--------------

Work should happen in feature branches in git, with pull-requests that the other developer approves and pulls in

#### Front End Nightmare:

-	Instead of Rails making HTTP requests, have jQuery make HTTP requests to backend and render using Handlebars
-	When PusherApp receives a new sshhh, render it automagically

#### Back End Nightmare:

-	When a new sshhh is posted, send an update to front-end using PusherApp
-	Log all API calls and make a maximum of 60 calls per minute. After which you'll return a 503.

Notes
-----

-   Backend will need to allow "CORS". Check out "rack-cors" to allow javascript
    ability to ask for JSON from a different domain.
-	You can add your requirements to a [Trello](http://trello.com/) board to see what remains to be done.
-	How to deploy a subdirectory to heroku [Notes](https://sndrs.ca/2013/11/15/deploy-a-subdirectory-to-heroku-as-an-app/)

```
git subtree push --prefix backend heroku master
```

Additional Resources
--------------------

-	[jBuilder](https://github.com/rails/jbuilder)
-	[PusherApp](http://pusherapp.com/)
-	[Pull Requests](https://help.github.com/articles/using-pull-requests/)
-	[Git Branches](http://gitref.org/branching/)
