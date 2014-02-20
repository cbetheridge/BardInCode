BardInCode
==========

Representing William Shakespeare's popular works in high-level programming code

- - -

When new programmers are being taught their first language, the process of learning a programming language is often compared to learning a spoken or written language. The goal of this project is to test the validity of that comparison by attempting to represent the works of William Shakespeare in programming code.

This does not mean reproducing the text, but reproducing the meaning of that text. An example

Romeo and Juliet
 SCENE I. Verona. A public place.
   Enter SAMPSON and GREGORY, of the house of Capulet, armed with swords and bucklers

Might be represented in python code as

 Class Verona(Place):
  self.occupants = []

 Class SceneOne(Scene):

  def Play(self):
   self.location = Verona()

   sampson = Person(name="Sampson", house="Capulet", armed=True)
   gregory = Person(name="Gregory", house="Capulet", armed=True)

   self.location.occupants.append([sampson, gregory])

We first setup that a Verona is a place that has occupants, and that a scene is a list of events that represents the story of Romeo and Juliet through state changes in the app. Note that I made no mention of swords or that Verona is a public place. That's intentional, by skipping these we are avoiding going down a rabbit hole of infinite object-oriented taxonomy, while still representing the core meaning: Sampson and Gregory enter the scene.

The goal of this project is EMPHATICALLY NOT to build a full programmatic representation of a written language or real life. Instead the goal is to test how well we can convey the core meaning through computer code, as a programmer reads it. When SceneOne is completly written, I should be able to take a debugger and step through the code. If successful, as I step through I should be able to understand the events that transpire in the work.


RISKS:
 - Death by design indecision. The possible ways of approaching the projects goals are innumerable, and could easily derail the project through.
 - Scope bloom. The above example is naive and an iceberg (I havn't defined Scene or Place, or Person yet) and unless scope is carefully locked down, the project can easily slip into taxonomy. The core question at every single step should be "Does this change significantly increase meaning? And is it absolutely neccessary?" Striking that balance between representation of the prose and completeness of meaning is playing a game of chicken with the edge of an abyss.

HOW TO HELP:
 1) BEFORE YOU EVEN LOOK AT THE CODE go (re)read the text. We're starting with Romeo and Juliet because it's popular. http://shakespeare.mit.edu/romeo_juliet/full.html Make some tea and have an evening of it. It's not that long, and Shakespeare is public domain.
 
 2) The beginning, dare I say most, of this project are going to be all about design and scope. What to represent  in code and what to skip. How to design a Scene object, and so on. It creates an unfortunet overhead, but reading through what's been established first will be benificial.
 
 3) Contribute opinions on the Wiki. For now the wiki will be the main method of communication. TODO(cbetheridge): Stub out the wiki to facilitate discussion.

When you do get to the code, we will be using git's issue tracker for bugs.
