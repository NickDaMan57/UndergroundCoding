---
layout: post
title:  "Behavior Track"
date:   2018-07-18 00:00:00
categories: Android-Dev
tags: NewProject
excerpt_separator: <!--more-->
---
I am attempting to build an Android app to help users log and keep track of their behaviors. The goal of this app is to help people who wish to instill or eradicate certain behaviors from their life.

This app will be gradual in its development, as I set out to learn the intricacies of Android development through modular programming. This means that I will attempt to add one functionality at a time, as I learn how to implement said functionality.
<!--more-->
## Final Version
The program, in its entirety, will have the following functions and features:

1. User-defined behavior creation will be saved to a database, either local or remote, as per user's choice.
2. There will be 3 main types of behaviors:
 1. Behavior
 2. Activity
 3. Emotion
3. Android notifications will prompt user for status of behavior. The user specifies the time for each notification. (ex: Prompt: Did you go to the gym today? YES NO OTHER)
4. The application will offer a graphical representation of user behaviors statistics through various charts.
5. User will be able to overlay charts.

## First Steps
As I set out to build this app, the first thing I will need to do is create an app that stores some form of user data to an app file. Because I will later change the data-storage scheme to a database, I will be using an interface to maintain funcitonality when the time for change comes.

After the file-saving mechanism is provided, the next step will be to display the data. Again, because this scheme will later be changed to a database one, an interface will be put in place to facilitate the transition.

The next step will be to implement an Android notification that prompts the user for input regarding a specific behavior. Notice that at this point the user is only able to work with **one** behavior at a time.

Only after I have achieved proper notification prompts will I attempt to implement multiple-behavior management.

For multiple-behavior management I will need to implement a list view (RecycleView) to display each data entry onto the screen. At this point there are many details to be analyzed, such as how the data will be displayed according to different behaviors. This may be a place of significant frustrastions and time consumption.

Once the list view is completed, I believe the most important next step will be to fix the notification scheme to reflect multiple-behavior as well (that is, each behavior gets its own notification prompt).

Having done this, the functional part of the program is complete and I am left with either adapting the app to a database and implementing cloud functionality, or stepping into the graphical statistic representatons, which I will need to do significant research before I even begin to talk about it.
