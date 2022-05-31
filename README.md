# Auth Workflow

Auth app for any project written using `Node Js` and `Express Js`

## Overview

 - Auth Workflow is basically a set `API` endpoints related to `authentication` and `authorization`. In this, I am using `JWT` strategy to authenticate and authorize the user for the action which user wants to perform.

 - Expressjs is a fast, unopinionated web framework for nodejs. It help in creating server-side web applications faster and smarter.
 
 ## Motivation
 
 - Using this authentication app, you can easily integrate authentication service with very minimal changes.
 - Rather than spending time on creating authentication logic and service, get on with the core functionality right away.

## Getting Started
Follow the following steps to run this application :-
`Step 1` :- Clone the repository.

    git clone https://github.com/rkg1007/auth-workflow.git


`Step 2` :- Install the dependencies

    npm install

`Step 3` :- Create the enviroment variables. The `env` should be placed in the root folder with the following variables :-

 - `MONGO_URI` (required) :- Connection string of mongodb database.
 - `JWT_SECRET` (required) :- Secret to sign the jwt token.
 - `JWT_ACCESS_TOKEN_LIFETIME` (required) :- Lifetime of jwt access token.
 - `JWT_REFRESH_TOKEN_LIFETIME` (required) :- Lifetime of jwt refresh token
 - `COOKIE_SECRET` (required) :- Secret to signed the cookie
 - `ACCESS_TOKEN_COOKIE_LIFETIME` (required) :- Lifetime of cookie which contains access token
 - `REFRESH_TOKEN_COOKIE_LIFETIME` (required) :- Lifetime of cookie which contains refresh token
 - `PORT` (optional) :- port on which application will run. If not provided then app will run on port 3000.

`Step 4` :- Running the app.

	# for development
    npm run dev
	
	# for production
	npm start


## Project Structure

| Name | Description |
| ------------------------ | --------------------------------------------------------------------------------------------- |
| **configs/**                         | contains the configuration files. |
| **controllers/**                | contains controllers files which maps http request to the service  |
| **routes/**               | contains router files which map http request to the controllers|
| **errors/**               |  contains the errors files |
| **middlewares/**             |  it contains custom middlewares used in project |
| **models/**               | contains the database models |
| **services/**               | it contains the files which runs the business logic on each http request |
| **utils/**        | contains some utility files                                                               |
| **node_modules/**         | Contains all your npm dependencies                                                       |     
| package.json             | File that contains npm dependencies          |

