---
layout: post
title: "Configuring Windows To Use Jekyll Part One"
description: "Configure windows to use Jekyll "
category: articles
tags: [jekyll, windows]
---

It really bugs me when I am trying to accomplish a task and not able to because my Windows machine does not comprehend what I am trying to do. I have been trying for days now to configure my Windows 8 computer to run Jekyll locally on my machine without much success. I have decided to try one more time to get it up and running. My programmer son said that I should use Linux for such a task and although I want to learn to use Linux eventually, my available time is limited with an ill parent, a teenage son and a "boss" who wants me to be working actively on GitHub every day.

So I have decided to give Windows one more try before moving on to Linux. Sigh!

![check ruby version](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1752_zps65b883d7.png)

The directions above to configure Jekyll can be found on [GitHub's](https://help.github.com/articles/using-jekyll-with-pages) website so hopefully I will get it working this time around. Although I know I have all the requirements it is good to follow directions so as to make sure that I am not missing a step. So here goes Step 1 and my result was...

![cmd ruby version check results](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1715_zpsb53cc03d.png)

Yikes!! That did not go too well. It seems I don't follow instructions well either. I typed  in ruby --Version when I should have typed ruby --version. Luckily Windows provided some help in that department and I was able to verify my Ruby version. Seems as though I have version 1.9.3p448 and I am guessing the date it was installed and some other folder information that I do not know what to do with quite yet. On to the next step.

![install bundler](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1826_zpsfce77f91.png)

Do not know if I actually have the bundler on my machine from my previous install so I am going to go ahead and install that.

![bundler install results](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1835_zps27d058f2.png)

So far so good. Nothing to do here but go on to step 3.

![step 3 install jekyll](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1839_zps9610c604.png)

Not too comfortable with the terminal so as per the instructions I created a file called the Gemfile ... just as it is written and put the line gem 'github-pages' and placed it where it needed to go as the pictures below confirm.

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1910_zpsc7b68951.png)
![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1911_zps3da087b4.png)

Now to run the command bundle install and then I should be "good to go" as per the instructions.

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1925_zps527b4347.png)

Although at the bottom of step number 3, had an example of the information you can put in the Gemfile, the instructions did not say that the web url for Ruby was important. Apparently it is from the above example. 

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1942_zps6d11a718.png)

So I made the necessary changes and it worked!Now reading the last line of the code it said that I should use 'bundle show [gemname] to see where  bundled gem is installed ... ok, good to know but how do I know which gem to look for ... better yet where do I find the name of such a gem. I want to know in case I need this information later but I did not know what to look for. 

Terminal to the rescue! I looked one picture up from this one and saw a message that said: 
> Could not find gem 'github-pages' ... on this machine.

That was a light bulb moment for me ... oh so the gems were all these name of "stuff" that it was installing. So kramdown was a gem and rdiscount was a gem and so on. If I wasn't such a novice I would know that!

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_1948_zps9bf789f5.png)

Yes! I want to know where github pages was installed ... you never know, I may need this information at some later date. Now for the fun part, getting Jekyll to serve my pages locally. Here goes, "bundle exec Jekyll serve" ...

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_2055_zps3f5030ae.png)

My server is running ... yeah! But what is that *[33mConfiguration file: none<-[0m* message anyway?

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/2013-09-30_2058_zpsea5f6a5a.png)

Noooo ... that's what! To be continued ...
