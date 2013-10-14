---
layout: post
title: "A Basic Function In Python"
description: "Define a function in Python and show an example."
category: articles
tags: [python, learn python, functions]
---


A function is, is a piece of code that you define that you can execute
later. You only execute the code inside a function when you call that function, and you can call the function more than once.

Before we actually type any code we have to think about what we want and decide what the function is going to do. A good way of doing that is to put it in a comment.

![Python Function Example](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-10-14_0954_zps8f9781a0.png)

A comment starts with a hashtag (#) The first line is called the header of the function. The second which is the rest of it is the body.

### What is the header? ###
The header tells you about the function, so it starts with the keyword `Def`. `Def` is short for define and you're telling Python that you want to define a new function.

I am going to compute the area of a triangle so I want to call my function triangle area. Next we have a parenthesis list of parameters and in this case this function takes two parameters, the base and the height of the
triangle. 

A functions can take zero or more parameters so, I can have zero, one, two, 100. How ever many parameters you need to compute what you are computing.
Also name your parameters in a way that is obvious to someone who is going to be using your program.

A colon has huge significance in Python, this means you're about to start a new block of code.

### The body of the function ###
The body of the function comes after the colon and is indented. It doesn't matter how much it's indented, but it does matter, it's indented by the same amount. When you stop the indentation, the block of code is done. 

Beginning at line 6 is where you call the function to make it work. It only executes when you call it.

You have a triangle - A1 that has a base of 3 and a height of 8 and you want to find the area. You call your function at lines 6 and 7. If your answer is 12, your program works. If it is something else, then there is something wrong with your code.

Trying your code with a triangle -A2 with a base of 14 and a height of 2 should produce an output of 14.

The example code below shows what happens when the parameters are empty that is - open & closed quotations ()
    
    |# prints hello, world!
     def hello():
    	print "Hello, world!"
    
    
    hello()  # call to hello prints "Hello, world!"
    h = hello()  # call to hello prints "Hello, world!" a second time
    print h  # prints None since there was no return value



Functions are extremely powerful and extremely useful and every program you
write will include functions. We have only scratched the surface here on
what you can do with functions. Don't forget the colon. Don't forget the indentation. And don't forget the return. These are critical pieces of the
functions. Hopefully, with a little practice. You'll understand and be able to use them.
