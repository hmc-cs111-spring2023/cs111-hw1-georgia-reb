# Context Free

##  Who is this programming language for?
For artists, but specifically those who want to experiment with context
free grammars.

## What is easy to do in this language? Why is it easy?
It is easy to create recursive images. This is easy because
a shape rule can include instructions to draw a shape and a recursive call
to the shape rule with updated parameters. The parameters can be created in
reference to the current values.

The idea for the language is inspired by a context free grammar, that is
why these recursive calls are very easy to create.

## What is hard to do in this language? Why is it hard?
There are only a few "primative shapes" defined in the language, including
squares, circles, triangles, or fills. Additionally you can use a path
declaration in order to create a new shape. Therefore, it is hard to use
any basic chapes that are not squares, circles or triangles because you need
to create them youself using the path declaration.

## How did you learn how to program in this language?
I looked at both the sample image and read the home page of the documentation.
Then I found that there were two lesson examples built into the program. I mainly
looked at the first lesson, which was very helpful to me.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

You create a program, then press render. The program looks to the startshape
commands, and then the context-free rules are followed to produce an image.

It is also important to note that the program will stop recursion when the shape
being drawn is too small to see.

## What do you think is interesting about the ContextFree program you wrote?
I created recursion within recursion! I wanted to make ominious stairs leading
up to the house, which I did using recursion. Additionally, I created a reursive
spiral of houses.
