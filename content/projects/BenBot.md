---
title: "Discord Bot"
date: 2024-04-20T15:21:07-04:00
draft: false
tags: ["Python","MongoDB"]
---


With this project I decided try something new. I wanted to create something me and other people would be able to use daily, that would provide utility. BenBot was my answer! BenBot is a discord bot that I created for my server with my friends. I decided to make my own bot so that I could have full control over how it worked, and I would be able to implement the features that I really wanted. I also thought it would be a fun learning experience, which it was. Additionally, if AI ever take over, it can't hurt to have one as my son. All jokes aside, BenBot is currently capable of:
- Recording cold takes
- Sending messages based on the current time
- Listening for keywords and taking actions based on them
- Saving messages to a database
- Grabbing messages from a database
- Using threads to track the current time, while still listening for keywords from users
- Silencing users
- Sending messages at random


![BenBot](/Discord.png)

The “cold takes” feature is currently the main feature of BenBot. It works by having a user respond to a message that they think will not age well. For example Bob may say the lions are going to win the superbowl this year and Alice may think that he is crazy. So Alice responds to the message with a date in DD/MM/YYYY format. That message is then saved to a database using MongoDB, with the date it is sent, and the cold take date. I used threading to have the bot check the time periodically, to allow the bot to still be capable of other features while waiting for the cold take date. At 1pm EST each day or upon wakeup, the bot calls the database and checks for any records where the current date matches the cold take date. The matches are pulled and are sent into the discord server, and then deleted from the database. Everyone can then see, sometime after the super bowl, if Bob was right, or if his take was cold. More recently I have added quality of life features, which force the user to have a proper input and will check if any takes were missed due to downtime.

BenBot can be called upon with commands as well, such as $roll. This command will send a random answer from a list of predetermined responses, acting as a magic 8 ball of sorts. Users are meant to ask questions along with the $roll, such as “$roll will the sun rise tomorrow?” and BenBot will answer.

Lastly, BenBot was started back in 2022, but I regularly update him with new features. BenBot has been great at providing funny moments for me and my friends, and is my favorite project I have worked on!
