# Express Exercises
The goal of these exercises are to become familiar with the basic concepts behind Express, in particularly how to route HTTP requests, and use middleware

## Get started
The first thing to do is to install Node, and NPM, which comes with it.  We will also need Git, so that we can obtain a copy of the exercise materials

### Installing Node and NPM

#### On MacOS and Windows
Download and run the installer from https://nodejs.org/en/
(alternatively, if you are on MacOS and have homebrew installed, you can type 'brew install node' on the command line)

#### On Linux
Probably the easiest way is to install node from your package manager.  Follow the instructions for your distribution here: https://nodejs.org/en/download/package-manager/

### Installing Git
You also need to make sure you have git installed.  Follow the instructions on the Git project's website:
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

### Clone this repository
On the command line, navigate to a suitable directory where you want to work, and use the 'Clone or download' option on the github repository page to clone the repository

https://github.com/leanjscom/express-exercises

## Exercise 1 - Basic Routing
This exercise is to practise creating some routes to handle incoming requests.

Have a look at the script 'index.js'.  It won't work at the moment because it is missing some code; add the missing code.  Once you have got it working, add another route to handle the URL '/plants', as per the instruction in the comment in the code.

Then add a route to handle getting a specific plant by ID, using route parameters.

If you have time, try adding some routes to handle other HTTP methods, such as POST, PUT, or DELETE; test them using cURL on the command line (POST is probably easiest to test like this)


## Exercise 2 - Using templates
You may have noticed that in Exercise 1 we used a lot of repeated HTML code.  One way to avoid this is to use a templating engine.  We will have a go using the templating engine Mustache.

### Task 2.1 Install the package 'mustache-express'

### Task 2.2 Correct the lines at the top of templating.js in which mustache is set up as the templating engine for the app

### Task 2.3 Rewrite the route for 'plants' to use Mustache partial templates, as per the route for 'animals'

### Task 2.4 Add your own templates and experiment with using them



### 2.  Initialise the project as an NPM package
On the command line, navigate inside this project, and set-up a new NPM package by typing 'npm init' and accepting the default answer at all the prompts

	cd express-exercises
	npm init

You will notice that there is now a package.json in the project

### 3.  Add express to the project
On the command line, from inside this project's directory, add Express using NPM.

	npm install express --save

You will notice that express has been added to package.json as a dependency

### 4.  Fix the index script
Have a look at index.js.  Try to use it by running 'node index.js' on the command line.
