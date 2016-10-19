---
layout: post
title:  "Citbike Routing Directions and Time App"
date:   2016-10-19 14:23:11 -0400
categories: web apps
bigimg: /img/citibike.jpg
---

**Currently a work in progress.**

This [app][citibike-app-link] is a functional website built to fulfill a need I had, providing a better way to route a user from a location to a destination using the NYC citibike network. The app has a simple front end built with Angular 2 and the Angular 2 CLI and utilizes bootstrap for simple styling.

The app submits data to a backend built using Node with Express that is deployed to Heroku. The backend uses the Google Maps geocoding API to take the users input and translate this to actual locations with latitude and longitude and sends this back to the user to confirm the locations. When the user then calculates routes the information is again sent to the backend where the nearest citibike stations for both the starting and ending location are found. The google distance matrix API is then used to give time estimates for various forms of transportation to the user. This includes walking, biking, driving, and citibiking - a combination of walking to the nearest station, biking between the stations, and walking to the final destination. This information is once again sent to the front end and displayed to the user. The user can then get routing information for the individual segments of transportation through the google maps directions API - this is directly handled on the front end.

This app was a learning exercise involving additional angular 2 features, simple animations, interactions between front and backend, nested angular 2 components, interaction with google maps apis, and more. There is potential room for future development to incorporate public transit, zip cars, car2go, and other combined transportation methods.


[citibike-app-link]: http://zebesta.github.io/citibike2/
