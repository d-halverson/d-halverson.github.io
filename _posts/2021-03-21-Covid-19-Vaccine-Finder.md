---
title: "Automating the Search for Covid-19 Vaccine Appointments at Walgreens"
layout: post
date: 2021-03-21 12:30
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Python
- Selenium
- Walgreens-Scraper
category: blog
author: drewhalverson
description: Published Walgreens-Scraper project to GitHub!
---


# Why did I create this?
As a break from school and work, I decided to make a small project that I could learn about a new topic (web scraping) while creating, and also create something useful. As finding Covid-19 vaccination appointments has been very difficult due to high demand and limited supply, I decided to create a Python script that will notify me when an appointment becomes available in a list of zip codes that I specified.

# How it works
Using the Python library [Selenium](https://selenium-python.readthedocs.io/getting-started.html), I learned how to interact with a webpage through Python code. The program I created simply iterates over a list of zip codes that I specify, and then types each one into the text box on Walgreens's website. Then, it reads the pop-up that appears as either "Appointments available!" or "Appointments unavailable". Once an appointment is found, I send a text message to my phone with a message that looks like this:
<img class="image" src="https://d-halverson.github.io/assets/images/appt-found.png" alt="Program demonstration image" width="500">
<figcaption class="caption">Appointment found message send by SMS.</figcaption>


Here is a quick demonstration of what it looks like when the program is running (running on zip codes near UW-Madison for testing purposes, but did not find any appointments during demonstration):
<iframe width="560" height="315" src="https://www.youtube.com/embed/JkJHz0Q2sAc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

Read more at: [GitHub Link](https://github.com/d-halverson/Walgreens-Scraper)
