---
layout: post
title: Installing Flask to Ubuntu Final
description: "Directions and Images for Installing Flask to Ubuntu."
modified: 2014-02-09
category: articles
tags: [flask, python, learning python]
---

Even after my previous install and its many errors I decided to continue right along to the next logical step which is to look for the basic *Hello World* application to test my Flask install.

I went to the [Quickstart page of Flask](http://flask.pocoo.org/docs/quickstart/#deploying-to-a-web-server) and there I found the directions for my first App.

    from flask import Flask
    app = Flask(__name__)
    
    @app.route('/')
    def hello_world():
    	return 'Hello World!'
    
    if __name__ == '__main__':
    	app.run()

Ok, they did not quite tell me how to go about making the file since the documentation was not written for novices.

I remember trying to create a file in Linux a while back and it said use *"touch"* to create an empty file, so I did that and named it hello.py as it said in the instructions. Then I used *"pico"* to edit the file and typed the above code. Now it was time for me to run the code to test my Flask installation. And ...

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2014-02-06_2358_zps07383f0a.png)

Yikes!! I am getting errors. Is it because Flask did not install correctly or did I make a typo in my python file? Here is what I typed into my python file.

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2014-02-09_1535_zpscb4ec3fc.png)

Does it look like what is typed in the code above? Well apparently I did think it was correct because I dismissed it and went on to make other decisions in trying to find out how to fix the Flask install.