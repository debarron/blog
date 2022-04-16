---
title: "Checking the NBA calendar as a web scrapping exercice"
date: 2022-04-12
tags: [dev, python, web-scrapping]
excerpt: "This is a cool way to start coding in Python"
---

I've always enjoyed playing and watching basketball, nature pointed me to the sport 
(I'm 1.9m, something like 6'2"). 
But I keep missing the NBA game broadcasts everytime, and by the time I realized this 
the game has already finish. 
So, I decided to put matters into my own hands and avoid setting up alarms and go for a
different software solution. That, and I needed a good hook for this post. 
So, TL-DR version *I built a web-scrapping script in Python to go and pull 
the games' calendar from the NBA official web site*.


## Before we continue
If you are following this post but have no Python coding experience or knwoledge, please go 
and visit the G.O.A.T. [Derek Banas in Youtube](https://www.youtube.com/channel/UCwRXb5dUK4cvsHbx-rGzSgw).
Here are some videos that'll help you get started: 
* [Python Tutorial](https://youtu.be/H1elmMBnykA)
* [HTML Tutorial](https://youtu.be/Ggh_y-33Eso)


## How I tackle this problem
In recap, I needed the game callendar from the NBA official web site.
Fortunately for me, NBA has an clear and friendly page to get this info.
So I visited the [NBA Official game schedule page](https://www.nba.com/schedule) and got
a feeling of what's there.

I realized we can look at the **CALENDAR** option to choose the month, also we can
select a specific **TEAM** from the league. 
Other option that we can choose is **BROADCAST REGION**, and if you live in Mexico
(like I do) you'll be very interested.

Now, I chose to monitor all the broadcasts of **Brooklyn Nets** games for next month in
Mexico.
After I picked **May, Brooklyn Nets**, and **Mexico** from all the options in the web site
we formed a new URL `https://www.nba.com/schedule/nets?cal=May&region=22`.
This tells us how we can communicate with this web site, and we can talk about that some
other time.
So, what I'll do next is take this URL with me and write a Python script that will
download all the HTML information from the web site, parse it, and get the game schedule.


## Let's code it




Any of these ring a bell? 
A straight forward way to show that you understand how web-pages are organized.
You want to automatize some tasks related to visiting, or checking a web page's content
You're bored and want to learn something new
You want to procastinate
You want to practice some pythonian ~magic~ logic

If not, then you have your own reasons.



## What do we need?
We have a program (a script in python)
We have a web page (can be more than one, it does not matter)
We have a behaviour that has to be automatize.
Then we have all the ingredients.

### Libraries
* Beutifulsoup, to handle html parsing and scrapping
* Response, to handle HTTP requests


## There ain't no such thing as a free lunch
I'm not in the hacker-know-it-all level, so
We have to look for patterns in the web-page and check how can we interact with them.

### Checking the URL
* Main page
* How does it look when I change the calendar
* How does it look when I change the team
* How does it look when I change the region

### Checking the content
* Look at the table with the standings
* Inspect the elements and get the class



## Modeling the behaviour
Think of this behaviour as a _function_ where
* Its **input** is an HTML page
* Its **output** is something we need for that page 

### Take it to the console
* Query and get info, double check if we got the elements right
* Keep the filters



## And here it is
The behaviour I want to automatize is the following

As it was mentioned before, this would be code in python.
We'll use the libraries A and B.
