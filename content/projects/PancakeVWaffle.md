---
title: "Pancake or Waffle?"
date: 2022-05-05T15:21:07-04:00
tags: ["Python","Selenium"]
draft: false
---
![Pancake V Waffle](/pancakeVwafflePlot.png)
![Pancake V Waffle](/PancakeVwaffleEval.png)

I wanted to learn more about machine learning and fill the gap in my knowledge the best I could, as I never got to take a dedicated class about the topic. This inspired me to create a program that would implement some basics of machine learning. I created a tool that labeled whether a picture was of a pancake or a waffle. The program achieves around 90% accuracy for the labeling. Due to having a relatively small data set, I used data augmentation to help avoid overfitting. 

While the program was relatively simple, the biggest lesson I learned is that the dataset is just as important as the algorithm used for training.

To help solve my dataset problem that I faced, I implemented a google image web scraper. The web scraper is able to download nearly all the images of a specified search term automatically by using Selenium. Using this tool allowed me to get a decent sized data set of around 700 images, and all I have to do is type in my search term.

Overall, while knowing the difference between a pancake, and a waffle is not world changing, I learned a lot. I was able to problem solve to find a solution to quickly and easily gathering data sets, and I created a tool that could classify pancakes and waffles with decently high accuracy. The main takeaway of this project for me was how I ran into a problem, and was able to solve it to create a system with the capabilities I needed.

