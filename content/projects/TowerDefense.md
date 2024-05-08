---
title: "Tower Defense Game"
date: 2021-04-30T15:21:07-04:00
tags: ["C++"]
draft: false
---

For the final project in one of my 300 level CSE classes at MSU, we were to create a simpler version of the popular Bloons Tower Defense Game. I no longer have access to the code, but I still wanted to talk about some features that the game had, and what I learned.

The game featured multiple levels, the layouts of which were contained in XML files. These files stored the tile type and location. The board was laid out as a grid, which enabled the pieces to be placed one by one to form a complete picture.

The gameplay featured users dragging and dropping unique towers, which detroyed balloons passing by. The goal of the game was to prevent the balloons from reaching the end of the levels pathway/track the balloons followed. Once all the balloons were destroyed, the game progressed to the next level.

The code behind this was a time based loop. Balloons would be spawned in periodically, and there was a list of towers that could be added to whenever a user added a new one. Each tower had a timer which determined when it activated. When activated, the objects shot out of them would be checked if they overlap with a balloon, and if so the balloon deleted and points awarded.

This logic of: The balloon spawned, then each tower visited, each towers projectiles checked for overlap, a timer for the tower checked to see if a new projectile should activate, then back to the start of the loop, continued until the round ended.

Implementing the different towers helped teach me about inheritance, because each tower had a location, but the capabilities were different and required the class to be extended upon.

The best part of this project was implementing our own tower, a Road Runner from Looney Tunes, which bounced back and forth across the screen quickly. For this, we won an award for creativity, and got to skip the final!