# help-demo
## Demonstration Client
This little console app connects to an ill-behaved (and very creatively nasty) server
as specified in acceptance criteria as a coding exercise. 
For security reasons the specifics of the server and 
acceptance criteria are not included in this repo.

###Installation
Make sure that you have Node.js LTS (8) and npm (5)
installed.  Clone the github repo onto your local machine.

`git clone git@github.com:wmaness/help-demo.git`

`cd help-demo`

Then install dependencies.

`npm install`

Because it is a terrible idea to have connection or security information on github, you will need to set three environment variables before executing the code.

`export help_demo_host=<1.2.3.4>` IP address of the server you want to connect to.

`export help_demo_port=<1234>` Port you want to connect to

`export help_demo_username=<MyUserName>` The username you want used for authentication to the demo server. (Limit 12 characters)


###Test
Mocha and chai are used for unit testing.  You can execute the tests using npm.

`npm test`

###Execution
To launch the app, npm to the rescue.

`npm start`

The application will prompt you with your options, and allow graceful disconnection.

###Logging
Application logs are being sent to loggly.com. Yes. I'm monitoring my process and spying on you.

