---
layout: post
title:  "Change Ringing"
date:   2016-11-28 19:53:12 -0400
categories: Python Flask
bigimg: /img/bells.jpeg
---
This project was a collaboration with [Myles Dakan][myles] during our time together at the [Recurse Center][recurse]. Myles had already created an interesting Python app for Change Ringing - a way to produce music with bells by ringing them in a pattern-based sequence. For more information see this [video][video] and [detailed explanation.][explanation] The app interprets change ringing notation in a variety of forms and automatically generates the music as well as its notation.


The functional python script was interesting, but no average user would be able to interact with it from the command line. We chatted for a bit and decided to work on "webifying" the application with a Python web framework I had been recently learning called [Flask][flask]. With a little bit of server side rendered Jinja HTML, some python backend design, and some refactoring and error handling work from Myles, we put together a simple website that lets users experiment with Change Ringing and hear a midi sample of the output. Users can generate their own content using change ringing notation that is standardized into an expected string on the backend. This app was a learning exercise to explore Python 3 based backend development with the Flask framework, Jinja, and Pillow with some bootstrap based CSS. The app is deployed to Heroku using Gunicorn.

<!--  
Expand upon how the data is dynamically rendered and sent, and it does not use a database
What I found interesting about making a project in flask
Talk more about the learnings
 -->


Check out the [Change Ringing Web Site][change-ringing] and give it a try! (**Warning:** This will take about 20 seconds to load for the first time as it has to wake up the Heroku Server) As always, if you have any comments or questions feel free to send them my way or take a peak at the [source][sourcelink] if you wish!

[change-ringing]: https://change-ringing.herokuapp.com/
[myles]: https://github.com/mylesdakan
[recurse]: https://www.recurse.com/
[flask]: http://flask.pocoo.org/
[explanation]: http://www.cccbr.org.uk/education/thelearningcurve/pdfs/200404.pdf
[video]: https://www.youtube.com/watch?v=3lyDCUKsWZs
[sourcelink]: https://github.com/zebesta/change-ringing
