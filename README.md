# Week-7-Homework

## Live Link: 
https://joycetio.github.io/Week-7-Homework/

## Overview: 
Create a train schedule application that incorporates Firebase to host arrival and departure data. Retrieve and manipulate this information with Moment.js. This website will provide up-to-date information about various trains, namely their arrival times and how many minutes remain until they arrive at their station. 

## Instructions: 
* Make sure that the app suits this basic spec: 
    * When adding trains, administrators should be able to submit the following: 
        * Train Name
        * Destination
        * First Train Time -- in military time 
        * Frequency -- in minutes 
        * Code this app to calculate when the next train will arrive; this should be relative to the current time. 
        * Users from many different machines must be able to view same train times. 

## Technologies Used: 
* Bootstrap CSS 
* Javascript/jQuery 
* Moment.js
* Firebase 

## Code Explanation: 
* Updates "Next Arrival" and "Minutes Away" every minute: 
```
 <meta http-equiv="refresh" content="60">
```
* First, I went to Firebase to get the configurations I needed to add Firebase to my web app. 
````
var config = {
    apiKey: "AIzaSyC1Z6zs6E-f7J1N3VXitLcHIEtyYZiOUi0",
    authDomain: "week7-homework-9289c.firebaseapp.com",
    databaseURL: "https://week7-homework-9289c.firebaseio.com",
    storageBucket: "week7-homework-9289c.appspot.com",
    messagingSenderId: "309439026834"
};
firebase.initializeApp(config);
````
* For this homework, I mostly used moment.js to get the current time, and format it the way I wanted to. By using moment.js, I was also able to find the difference in minutes, and find out when the next train will arrive. 
