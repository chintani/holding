---
layout: post
title: "Numbers &amp; Arithmetic Expressions In Python"
description: "Learn about numbers and arithmetic expressions in python."
category: articles
tags: [python, learn python, numbers, arithmetic expressions]
---

On your journey of learning how to program in Python. 
Today's lesson is fairly straight forward, you've probably seen some of this in middle school and high school 
algebra.
 
We're going to give it some data, in this case, numbers and we're going to ask it to do some operations. 

let's talk about numbers and their arithmetic expressions. 
So to begin, let's just dive right in and have Python print out some numbers. So let's print 3 and -1 and 3.14159 and 
maybe -2.8. So if I hit Run here, sure enough out 
come those numbers.

in Python there are actually two types of numbers. There's kind of sign whole numbers, things like 3 and -1. And then there are decimal numbers that kind of have fractional parts and always have a decimal point. 

And in Python those sign home numbers are called ints or integers and kind of the decimal numbers are called floats or floating point numbers. And if you are ever in any doubt about kind of what kind of number you are working with. There is a function in python which can actually tell you what type of number you are working with is called type. 

floating point numbers are only an approximation to a decimal number. For example, when you do 1 divided by 3, 
you expect the decimal representation of something like 0.33333333 with 3 peats forever. 

So what happens inside Python is they, they represent floating point numbers with about 15 decimal digits of accuracy. So anything beyond that gets thrown away. So, in particular, occasionally when you're doing arithmetic operations using floating-point numbers. You're going to get answers of the form four point and a bunch of zeroes and then maybe a three at the end. What you're seeing here is called, something called floating point error. Whereas Python is doing the computation. It can't do the exact, precise operation which you're specifying. It can't compute pi to the last decimal point, or one-third to the last decimal point. So, it has to do some approximation.


### arithmetic operations ###

the arithmatic operators you have available to do 
computations in Python.  here's a list of, kind of, basic 
arithmetic operators, we have plus, minus, times, division, power, it's fairly straight forward. 

one operator that you should pay attention to in Python is division. So, the, the way the division operator works in Python 2 is different in the way it works in Python 3. 

In Python 2, if one of the operators is a floating point number, then the result of division is also a floating point number. And it approximates the actual division. 
So, for example, I could say print 1.0 divided by 3 or 5.0 divided by 2.0 or minus 7 divided by 3.0. And what would come out when I run that is what I'd expect kind of a decimal approximation of 1 3rd, 5 halves and kind of minus 7 thirds. notice at 5, both the operators are actually integers. 

And we'll actually talk about division 
more later on, when we talk about 
remainders. And we'll have the second operator 
called, slash, slash is explicitly integer division. 
All right, we know about numbers, we know about arithmetic operators. Now, we're ready to build arithmetic expressions. 

So, the idea is fairly simple. An arithmetic expression is either a number or it's an arithmetic operator applied to two arithmetic expressions. 

In which we should do operations when we are taking kind this linear version of an expression trying to think about in terms 
this kind of recursive definition. So it says that we are value an expression, we should always do parenthesis first and then after that we should always do exponentiation next. Then we should go through and do multiplication and division, M and D. And in fact, those have equal precedence. So if we have a sequence of those, we just do em from left to right. And then finally we do addition and subtraction last. 
