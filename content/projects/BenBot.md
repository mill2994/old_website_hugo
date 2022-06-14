---
title: "Discord Bot"
date: 2022-05-20T15:21:07-04:00
draft: false
tags: ["Python","MongoDB"]
---
![BenBot](/Discord.png)

With this project I decided I was going to branch out from the types of projects I have typically worked on. I wanted to create something me and other people would be able to use daily, that would provide utility. BenBot was my answer! BenBot is a discord bot that I created for my server with my friends. I decided to make my own bot so that I could have full control over how it worked, and I would be able to implement the features that I really wanted. I also thought it would be a fun learning experience, and that it was. Additionally, if AI ever take over, it can't hurt to have one as my son. All jokes aside, BenBot is currently capable of recording cold takes, sending messages at specific times, listening for and responding to key words, saving to and accessing a database, using threading to keep track of date and time, and responding to specific users or channels, with updates coming regularly.

The “cold takes” feature is currently the main feature of BenBot. It works by having a user respond to a message that they think will not age well, with a date in DD/MM/YYYY format within the reply. That message is then saved to a database using MongoDB, with the specified date and message as values. Next, I used threading to have the bot check the time every second, to allow the bot to still be capable of other features while checking the time. If the time is 1pm EST, I then have the bot call the database and check for any records with the current date, and the matches are pulled. Any entries gathered are sent into the discord server, and then deleted from the database.

BenBot also can be called upon with commands, such as $roll. This command will send a random answer from a list of predetermined responses, acting as a magic 8 ball of sorts. Users are meant to ask questions along with the $roll, such as “$roll will the sun rise tomorrow?” and BenBot will answer.

Lastly, BenBot is capable of 24/7 uptime by using UptimeRobot to ping the bot and Replit to host the program.
