---
layout: default
title: "Checking the NBA calendar as a web scrapping exercice"
category: dev
---

I've always enjoyed playing and watching basketball, nature pointed me to the sport 
(I'm 1.9m, something like 6'2"). 
But I miss the NBA games broadcast everytime, and by the time I realized the game has
already finish. 
So, I decided to put matters into my own hands and avoid setting up alarms and go for a
different software solution. That, and I needed a good hook for this post. 
Then, TL-DR, we're building a web-scrapping script with Python to pull the game's calendar
from the NBA web page.

I assume that we have basic knowledge in Python, and HTML. Otherwise, you can always find
the great [Derek Banas in Youtube](https://www.youtube.com/channel/UCwRXb5dUK4cvsHbx-rGzSgw),
he's an amaizing bootstrap
* [Python Tutorial](https://youtu.be/H1elmMBnykA)
* [HTML Tutorial](https://youtu.be/Ggh_y-33Eso)


## Why do we need this?
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
