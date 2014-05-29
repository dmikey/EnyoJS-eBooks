The First Hour


Setting up your environment
=====================================

There are only a few tools that you will need through out this quick journey! Here they are:

* Text Editor of preferred flavor (if you are brand new to development, I recommend [brackets](http://brackets.io/), it is free and for Windows, Linux and OSX).
* For the duration of this book series, Chrome developer tools will be referenced. I recommend downloading the latest version of Chrome browser for your OS.
* The "Tools" download appendix from this repository. These supplemental files will be aid you in preparing to use Enyo on the web. My custom bootplate provides production ready minified versions of Enyo.
* 24 hours!

For the remainder of this hour, we will cover some concepts, and theory about using Enyo. In the next hour we will rapidly move into assembling our application. Don't worry about remembering all of these, we will review them when we encounter using them.


The concept of the ViewController
=================================

The idea of a View Controller, is that we abstract the graphical representation of the application, away from the a data representation of those graphics.

You can think about the View Controller as a sandwich artist. They assemble the ready made toppings, into a complete sandwich for you to use, the person assembling the sandwich does not need to know about how all of the toppings were prepared, they are available to assemble into a sandwich. The artist is only concerned with making the sandwich fit the toppings, and putting it into a nice looking wrapper.

The concept of the View
=======================

The idea of the View, is that, it is an abstracted representation of underlying data in a graphical form. It may contain tool-bars, buttons, repeaters, lists, and other widgets like; sliders, zoom controls, maps, and input boxes. These are the bits that make up the look and feel of the application.

This view is essentially the wax paper wrap that is going to surround the sandwich when it has been built. The wrap does not really know what kind of sandwich it will hold. We have a loose concept that the sandwich needs to be within the dimensions of the wrap for the two to work together. This is similar in the way we abstract interactions between the View and the ViewController.

The concept of the Controller
=============================

While the idea is nearly identical to that of the ViewController, the difference is that while a controller can also drive a view, it is also suited to abstract tasks away from the application.

We can use these to control other aspects of our applications that do not necessarily fit into other paradigms. We can control a variety of disconnected business logic that can be shared across components.

The concept of  the Model
=========================

The model is a representation of data. You may be thinking right now, that representation could be overkill for the dream application you have in mind. But models can be very flexible and aid the developer is dynamically driving the application without much programmed interaction.

For the beginner, grasping the concept of data binding can alleviate the frustration and worry of knowing deep JavaScript.

The concept of a Collection
===========================

A collection holds a bunch of models. Collections allow us to group together, a mostly repetitive collection of data.

This may sound boring, but later during exercises we will see how we can use a collection to drive the User Interface bits of our application, alleviated extra work we would otherwise need to do.

The component, our building block
=================================

The component is our sole building block in EnyoJS. Everything is derived from a component, even most of the Enyo controls - are them self Enyo components.

In Enyo we use components, to not only build our application, but to also build other components. Enyo is like a brick building set, components can be nested inside each other, creating new components, or combining components together in a layout.

What is a kind?
===============

There is a general term when it comes to Enyo. The kind. If you are a classical programmer, you can think of a kind directly as a class. The switch is general keyword reservation semantics.

Kinds represent the definitions of objects we want to create. A button is a kind, so an image. We can create our own kinds, or using Enyo's inheritance, we can borrow from another kind.

Why enyo.kind is important
==========================

Enyo uses a major recurring method call, enyo.kind. It's one of the most important calls in the framework. This method is known as a constructor factory.

What this means is that when we create a kind definition, Enyo does not actually create an object that occupies memory. We can feel free to create (with in reason) a multitude of different kinds. While these definitions do create new objects, they are not fully recognized instances.