#Android Assessment Tasks

Programming languages: Java and/or Kotlin

**Task 1** 

Having two JSON: **rooms.json** ([https://api.myjson.com/bins/1eyhi8](https://api.myjson.com/bins/1eyhi8)) and **person.json** ([https://api.myjson.com/bins/19b2z4](https://api.myjson.com/bins/19b2z4)). 

Every item in **rooms.json** describes its center coordinates (lat, lon), radius and security access level (integer values 0, 1, 2, ... ).

Object in **person.json** describes a person's name, position (i.e. "engineer" or “assistant” etc), url of profile picture and personal security access level (integer values 0, 1, 2, ... ).

Also there is a condition of unstable internet connection, which means both JSONs should be somehow persisted into local device storage (e.g. as DB records). If connection is present, the app should fetch JSONs from the web, otherwise fetch data from the local storage.

The app’s objectives:

* To display person profile info (picture, name, position, access level)

* To detect whether the person is in radius of the restricted room. 

            ***_isRestricted = person.level < room.level_**

* If in radius then display alert warning (e.g. Toast or Snackbar)

   

**Task** **2** 

Given rectangular area where longitudinal axis is parallel to the equator, and its center coordinates (Latc, Lonc), width (W) and length (L) are known.

Latc = 1.180054

Lonc = 103.417785

W = 80 meters

L = 240 meters

You need to place a set of inscribed circles (R = W/2) and register each of them as a fence area.

Hint: 

Use the quick and dirty estimate that 111,111 meters (111.111 km) in the y direction is 1 degree (of latitude) and 111,111 * cos(latitude) meters in the x direction is 1 degree (of longitude)

![alt text](readme.res/ship.png)

  

The app’s goal is 

-To detect whether device is not within any of fence areas (e.g. out of rectangular area) and display alert warning (e.g. Toast or Snackbar).

Hint: 

You can use one of

-Geofencing [https://developer.android.com/training/location/geofencing](https://developer.android.com/training/location/geofencing)

-Awareness [https://developers.google.com/awareness/android-api/fence-register](https://developers.google.com/awareness/android-api/fence-register) 

-or any other API of your choice.

## Notes:

App should consist of 2 screens (Activities or Fragments - up to your choice), one screen per task.

Happy coding!

