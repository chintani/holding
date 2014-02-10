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