---
layout: post
title: "Troubleshooting a Detached Head"
description: "An example of a detached head and trying to fix it the novice way."
category: articles
tags: [git,github, detached head]
---

As with any novice trying to learn anything on your own you are going to run into problems --a lot. My latest adventure is when I deleted a couple of files that I did not want and then tried to commit my changes to Github.

I got a "Detached Head" warning. Now I am basically trying my best to navigate this 'Git thing' and now I have a 'Detached Head?'
 
I began my quest to figure out what was a detached head yesterday and with a little help from my son in clarifying a few things I am attempting to troubleshoot my own detached head problem. The picture below are screen shots I took of my 'Learn To Build Android Apps Repo' and even though everything is still a little foggy in what I need to do I am more knowledgeable today than I was yesterday to tackle this problem, so here goes!

![](http://i1205.photobucket.com/albums/bb424/cybercorp/GitHub%20Images/Github%20Holding/2013-10-12_1343_zpsa6bb1b30.png)

The areas that I will be looking at are these four, indicated by the arrows drawn. At HEAD(10) we have a clone to my computer (local machine) from GitHub the (remote machine). Head(9) seems to be where I run into my first "HEAD" problem. Head(8) shows that I did some sort of "[rebase](http://git-scm.com/book/en/Git-Branching-Rebasing "Rebasing on the git-scm book")" operation, again a little foggy on the details at to what I actually did as none of this was done from the command prompt but from me actually making changes on my computer and or GitHub. 

Incidentally my son tells me to STOP doing that because I am just making my learning more difficult than it needs to be. Since I am a visual learner (I need my pictures & windows) I will comply only partly! 

Moving on ... I did a [rebase](http://git-scm.com/book/en/Git-Branching-Rebasing "Rebasing on the git-scm book") and then went to `refs/heads/master`. Again, I was at a loss for what that meant so I went to the Git book again. Found and article on [References](http://git-scm.com/book/en/Git-Internals-Git-References "Git References") which is what "ref" stands for. So as a recap for me HEAD(10) is a clone of my repo on GitHub, HEAD(9) was me moving the "HEAD" from the master branch to a commit in that same branch a "README" file. HEAD(8)The rebasing occurred because I created and committed the file online at GitHub (I am guessing) and then returned the HEAD to master.

HEAD(7) Moving from master to origin master, in effect moving from git on my computer to git on GitHub. My next move was at HEAD(6) where I went to that commit "README" file again. I know this because the checksum (the long alpha number beginning with a3c772f) is the same from HEAD(9). I moved from that commit to ??? my screen shot does not say, so I will have to find out later by some other means that I have not learned yet. HEAD(5) was a commit in which I deleted the gruntfile and made changes to post Markdown and HTML pages. I moved from that commit to ???

HEAD's(4),(3), (2),and (1) is switching back & forth from branch master & ph-pages and vice-versa. My final HEAD(0) is a commit of deleted file theme-setup.

The question I now have is what happened when I checked out commit 0bb1fff and a3c772f? The answer to the question I will pursue at a later time to see if they are the cause for my Detached Head problem.

What I learned from this exercise is that commits should me made when the HEAD is at a branch. When a checkout of a commit is made it produces a Detached Head and I should not try to make a commit of any kind when the HEAD is not at a branch or it will put me in a Detached Head Status. 