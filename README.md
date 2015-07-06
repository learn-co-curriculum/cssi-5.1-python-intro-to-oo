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
+ class statement establishing a new class called Musician
+ members of the class Musician are defined with the __init__() method, whose first argument is self, followed by whatever additional arguments you choose.
+ within the __init__() we have our instance variables assigning our arguments.

Now we have our blueprint for our Musician.

Let's create some Musicians, some instances of the class object. We do that through **instantiation**, which means through calling the class, like we would call a function. We can give each new instance it's own name and genre.

For example:
```python
beyonce = Musician('Beyonce' , 'R&B')
```
We can make as many instances of Musician as we want. They’ll all be added to our class of Musicians.

The arguments we add to our class are descriptors that allow us to add more data to our objects, the methods we add to the class provide actions for our objects to execute.

You could continue to add arguments and methods to this class to add more information and specificity to each instance of Musician that you create.

**PARTNER PROGRAMNING**:
Great! Save your musician.py file for now. With a partner, try creating your own class and instantiating some objects in that class! Let’s put these blueprints to work inside their little factories and churn out some objects!

What did you make a class of, what were the arguments you used to define your class?

**Adding Methods:**
+ Let's add a method to our Musician class that will describe an instance of musician for us.

```python
class Musician(object):

    def __init__(self,name,genre,fav_album):
        self.name = name
        self.genre = genre
        self.fav_album = album

    def description(self):
        print "Hey, my name is {0}, I make {1} music. Check out my album {2}." format(self.name, self.genre, self.album)

kanye = Musician('Kanye', 'Rap', 'Yeezus')
```
+ Let's call that method:

```python
kanye.description()
```

+ Let’s add another that tells us if the musician is currently recording. We’ll need a new method and a new argument for our object that has a boolean value:

```python
class Musician(object):
    def __init__(self,name,genre,fav_album):
        self.name = name
        self.genre = genre
        self.fav_album = album

    def description(self):
        print "Hey, my name is {0}, I make {1} music. Check out my album {}." format(self.name, self.genre, self.album)

    def is_in_studio:
        if self.recording:
            print "Yo, I'm in the studio recording some fresh tracks! Holla at me later!"
        else:
            print "Hoping to get in the studio soon, I know you are jonesing for new material!"


kanye = Musician('Kanye', 'Rap', 'Yeezus', True)
```

+ Let's call our new method on our instance:

```python
kanye.is_in_studio()
```
**PARTNER PROGRAMMING**:
Try adding a couple methods of your own to the class you made earlier. What actions make sense for the class of objects?

#Conclusion:

As you can see, there is more than one way of designing your code. There is a lot more that can be learned about Classes and the advantages working within this structure can provide, if you are interested you can continue learning about Object Orientation on your own. For now, familiarity with class structure for Python will be useful to us next week when we get into learning AppEngine. We’ll see python class again there.
