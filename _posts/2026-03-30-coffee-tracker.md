---
title: "Creating Untappd for Coffee with AI"
layout: post
date: 2026-03-30 11:13
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Coffee
- AI
- Google Antigravity
- Mug Shot
category: blog
author: drewhalverson
description: Creating a website to share and track your favorite coffees.
---

# What is Mug Shot?
MugShot is a coffee social media website that allows me to track the coffees I have, inspired by [Untappd](https://untappd.com). With the help of AI, I was able to quickly get a first version of this up and running. Now, I can share the coffees I drink with my friends, see what nearby cafes others are enjoying, and more.

# Some of my Favorite Features

## Feed
<img class="image" src="https://d-halverson.github.io/assets/images/coffeetracker/feed.png" alt="Coffee feed" width="500">

Infinitely scrollable feed of you and your friends' coffee posts.

## Nearby Cafes
<img class="image" src="https://d-halverson.github.io/assets/images/coffeetracker/nearby-cafes.png" alt="Nearby Cafes" width="500">

Google Maps powered map of nearby cafes, with the average user rating and number of checkins (posts).

## Search Coffees
<img class="image" src="https://d-halverson.github.io/assets/images/coffeetracker/search-coffees.png" alt="Search coffees" width="500">

Search and sort the database of coffee beans to discover new coffee beans. The same functionality works with coffee roasters, cafes, brew methods, and coffee grinders.

## Profile Pages
<img class="image" src="https://d-halverson.github.io/assets/images/coffeetracker/user-page1.png" alt="Profile page" width="500">

Users can upload their own profile and banner pictures, set a bio, and view stats of their lifetime coffees.

<img class="image" src="https://d-halverson.github.io/assets/images/coffeetracker/cafes-visited.png" alt="Cafes visited by user" width="500">

Similar to the nearby cafes page, but specific to a single user. It shows all the cafes you have visited in the world.

<img class="image" src="https://d-halverson.github.io/assets/images/coffeetracker/user-page2.png" alt="Profile page rating distribution chart" width="500">

Scrolling down more on the profile page, an emoji is present that changes based on how many coffees the user has drank in the past 12 hours. Also, a rating distribution chart of the user's ratings is shown.

# How was it built?
The backend (Go) and frontend (React) are both hosted in GCP, although the SQL database lives elsewhere due to free tier limits on a true SQL database in GCP.

It's using these products in GCP:
- Google Cloud Run: hosting the backend api and frontend
- Google Cloud Storage: for saving user images
- Google Maps Platform / Places: For generating the Google Maps and receiving data about cafes.

# Using Google Antigravity
I chose to use [Google Antigravity](https://antigravity.google) as my AI coding platform over others, because it has generous rate limits and is very similar to Cursor. 

# Future plans
I am continuing to improve performance and add features to the website, and I would like to create a mobile app version as well. This is part of the reason I chose to write the website in react, to make the conversion to a mobile app easier in the future. Eventually, I would like to open the site for more users; I will write another post here when the time comes.
