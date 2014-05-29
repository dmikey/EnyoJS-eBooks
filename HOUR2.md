The Second Hour

Let's build something awesome
=============================

You should now be ready to build something awesome. In the last hour we explored some general theory of Enyo, and some basic MVC (Model View Controller) theory. Do not worry if you can not remember it all. We will review those topics as we need them.

Now to introduce you to our project. What I have chosen to assemble for this series, is a Location aware, Locals application. We will utilize Yahoo! Query Language, and Yahoo! services to power our application. We will build a web application, that can be opened with any modern browser. We will include location away APIs, that will allow us to determine the user's location, and provide feedback.

Enyo has amazing portability. An application can be written to support modern web browsers from IE8 and later. Enyo can also be wrapped in web view containers like Apache Cordova, and can then be deployed through "App" stores, and ready for offline use.

Getting Started, our first code
===============================

The first component we are going to build is going to be our general UI chrome. We will start with the chrome of the application, so that we can quickly build something that will be gratifying. 

Lets create a folder that will hold our project. Through out the rest of this series this project folder will be refereed to as "our_project".

In "our_project" folder, we will make a new ".json" file, "deploy.json".

What is "deploy.json"? This file is used by the vanilla Enyo build process, to determine locations and included libraries that are needed to build an application.

Inside of the deploy.json we need to specify some information about how our application will be digested. For the purpose of this app, we will only need a simple reference to our entry package.js file.

	{
		"packagejs" : "source/package.js"
	}

There are many other options that can be included here. Such as a path to libraries, specific Enyo locations, and even assets.
