---
layout: post
title: "Hello Again VNC"
description: "Configuring a VNC client to use with Linux created on Digital Ocean droplet."
category: articles
tags: [vnc client, digital ocean, droplet, linux]
---

In my last post I successfully installed A VNC to my Linux droplet on Digital Ocean. However, by the time I got finished with Step 5 and successfully connected to the server, I managed to mess it all up to the point of no return ...(for a novice that is).

It started when I decided to follow the instructions beginning with:
> Recommended Step - Secure your VNC server session with encryption.

Well because I am using Bitvise Tunnelier to connect to the droplet and it is a SSH Client with tunneling capabilities ... hence the name I decided there was no sense in me following the instructions for connecting with *putty*. Needless to say that my way did not work so now I have to find a way to remove it all and start from scratch.

I went digging on the web for code to remove what I had installed and I came up with this:
    
    `apt-get -y remove ubuntu-desktop tightvncserver xfce4 xfce4-goodies`
Which uses the same argument I did in the first place but instead of the word "install" I have the word "remove. On doing that I produced these results:
# Place Image Here #
I am very encouraged by the results, seems smooth and no errors. Now I will attempt to do the install over again. I will not be putting snapshot of this process this time around because it was already documented in my post entitled [Hello VNC](http://hello-vnc), please see that post for a walk through.

After redoing the steps I was still unable to connect to the VNC until I started comparing the messages from the snapshots I took from my prior install on 10/04/2013.

