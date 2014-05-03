The First Hour
Setting up my environment
=====================================

There are only a few tools that you will need through out this quick journey! Here they are:

* Text Editor of preferred flavor (if you are brand new to development, I recommend [brackets](http://brackets.io/), it is free and for windows, linux and osx).
* For the duration of this book series, Chrome developer tools will be referenced. I recommend downloading the latest version of Chrome browser for your OS.
* The "Tools" download appendix from this repository. These supplemental files will be aid you in preparing to use EnyoJS on the web. My custom bootplate provides production ready minified versions of EnyoJS.
* 24 hours!

For the remainder of this hour, we will cover some concepts, and theory about using EnyoJS. In the next hour we will rapidly move into assembling our application.


The concept of the ViewController
=================================

The idea of a View Controller, is that we abstract the interaction needed with the Graphical portions of your application, with the Data representation of those graphics.

You can think about the View Controller as a sandwich artist. They assemble the ready made toppings, into a complete sandwich for you to use, the person assembling the sandwich doesn't need to know about how all of the toppings were prepared, they are available to assemble into a sandwich.

The concept of the View
=======================

The idea of the View, is that it is an abstracted representation of underlying data in a Graphical GUI form. It may contain Tool-bars, Buttons, Repeaters, Lists, and other widgets like; sliders, zoom controls, maps, input boxes.

This view is essentially the wax paper wrap that is going to surround the sandwich when it has been build. The wrap doesn't really know what kind of sandwich it will hold. We have a loose concept that the sandwich needs to be within the dimensions of the wrap for the two to work together. This is similar in the way we abstract interactions between the View and the ViewController.

The concept of the Controller
=============================

While the idea is nearly identical to that of the ViewController, the general difference is that while a Controller can also drive a View, is can be suited to generic tasks that you want to abstract away from the application. We can use these to control other aspects of our applications that do not necessarily fit in other places. We can control jobs, or a variety of disconnected business logic that can be shared across components.

The concept of  the Model
=========================

The model is the representation of your data. You may be thinking right now, that "data" could be overkill for the dream app you have in mind. But models can be very flexible and aid the developer is dynamically driving the application without much programmed interaction. For the beginner, grasping the concept of data binding can alleviate the frustration and worry of knowing deep JavaScript.

The concept of a Collection
===========================

A collection holds a bunch of models. Collections allow us to group together, a mostly repetitive collection of data. This may sound boring, but later during excersizes we will see how we can use a collection to drive the User Interface bits of our application, alleviated extra work we would otherwise need to do.