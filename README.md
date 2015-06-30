---
tags: cssi, python, OO, classes, methods, variables
level: 2
languages: python
---

#Object Orientation for Python: Creating Classes

#Objectives:

+ Get an intro to Object Orientation in Python
+ How to write a class with instance variables and methods.

#Motivation
As a programmer you have different design choices you can make for structuring your code. Object Orientation is a way to organize, manipulate and store your data. It’s a design pattern that provides a way of building new objects - say all the alien enemies in a video game, Sim people in the sims, cars in Grand Theft Auto, users of Facebook - by making programs that are "factories" that standardize how the objects are made.

To generate new instances(versions) of an object we create something called a Class. The Class allows us to create a template for the objects we want to make. The template can then be tailored without having to recreate all of the code for each new instance of the object. Class syntax will give us a new way to organize and write our programs.

#Creating A Class
A class has this basic structure:
```python
class ClassName:
  'Optional documentation'
  class_suite
```
+ A class includes a **class statement** defining the name of the class, followed by the stuff that defines the attributes and actions of the members of that class - **methods** and **arguments**.
+ Class names should always be capitalized.

Let's make music!

Write a class that will allow us to create Musician objects.

```python
class Musician(object):

    """A class that creates awesome musicians!"""

    def __init__ (self, name, genre):
        self.name = name
        self.genre = genre
```
Now we have our blueprint for our Musician, but we haven’t created any actual musicians yet. To do that we need to create instances of our class, these instances are our objects. We do that through instantiation, which means through calling the class, like we would call a function. We can give each new instance it's own name and genre.

(Need to add the rest)
