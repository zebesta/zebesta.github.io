---
layout: post
title:  "NYC Bicycle Crash Map"
date:   2016-07-28 14:12:11 -0400
categories: android apps
bigimg: /img/BikeFeatureGraphic.jpg
---
NYC Bicycle Crash Map is an Android app to visualize motor vehicle crashes involving cyclists in New York City. This app is built using [information][nyc-data-link] provided by NYPD under the NYC Open Data Initiative. The goal is to show this data in a user friendly, familiar, and intuitive way so that cyclists can make informed decisions about the roads they take on their travels throughout the city. The controls are pretty self explanatory with the option to show either killed and/or injured cyclists and select the dates for the crashes to display. I'd love to hear any feedback and the app and am open to any ideas you would like to see added to the interface or application.

Check out the [NYC Bicycle Crash Map App][nyc-bike-crash-app] in the play store and give it a try! If you have questions, feel free to send me an e-mail. In the mean time, stay safe out there, NYC.




**Some technical information:**  This app pulls from the API to a locally stored SQLite database for faster access to the relevant data. This data is updated by a background service for the initial database population when the app is first opened and will update once a day to ensure the lastest data is always available. The data points are dynamically clustered and rendered based on the viewable area displayed on the map and density of markers to limit the total number of points to render and increase UI performance. The markers use a custom icon that distinguishes between injured and killed cyclists when they pop out of the clusters - black for killed and red for injured.

[nyc-bike-crash-app]: https://play.google.com/store/apps/details?id=com.wordpress.chrissebesta.nyccyclemap
[nyc-data-link]: https://data.cityofnewyork.us/Public-Safety/NYPD-Motor-Vehicle-Collisions/h9gi-nx95
