---
title: "Discord Bot"
date: 2022-05-20T15:21:07-04:00
draft: false
tags: ["Python","MongoDB"]
#featured_image: "/test.jpg"
---

BenBot is a discord bot that I created for my server with my friends. I decided to make my own bot so that I could have full control over how it worked, and I would be able to implement the features that I really wanted. Plus, if AI ever take over, it can't hurt to have one as my son. All jokes aside, BenBot is currently capable of recording cold takes, sending messages at specific times, listening for and responding to key words, saving to and accessing a database, using threading to keep track of date and time, and responding to specific users or channels, with updates coming regularly.

The cold takes feature is currently the main feature of BenBot. It works first by a user responding to a message, that they think will not age well, with a date. That message is then saved to a database using MongoDB, with the specified date. By using threading to keep track of time, so the rest of the features are not frozen, the bot waits for until 1pm then checks the date and pulls all the database entries with the same date. Any entries gathered are sent into the server, and then deleted from the database.

Lastly BenBot is capable of 24/7 uptime by using UptimeRobot to ping the bot and Replit to host the program
