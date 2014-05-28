The Second Hour

Let's build something awesome
=============================

You should now be ready to build something awesome. In the last hour we explored some general theory of EnyoJS, and some basic MVC (Model View Controller) theory. Do not worry if you can not remember it all. We will review those topics as we need them.

Now to introduce you to our project. What I have chosen to assemble for this series, is a Location aware, Locals application. We will utilize Yahoo! Query Language, and Yahoo! services to power our application. We will build a we app, that when opened with any modern browser, with location away APIs, will allow us to determine the user's location, and provide feedback.

A side note, EnyoJS is powerful, and has awesome portability. While a new application developer's goal is to move that app to Android, iOS, there are many ways to accomplish this. I will not be explaining them in detail in this series, but check the appendix for reference to where those materials can be researched.

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

