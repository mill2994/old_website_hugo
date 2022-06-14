---
title: "Pancake or Waffle?"
date: 2022-05-05T15:21:07-04:00
tags: ["Python","Selenium"]
draft: false
---
![Pancake V Waffle](/pancakeVwafflePlot.png)
![Pancake V Waffle](/PancakeVwaffleEval.png)

I wanted to learn more about machine learning and fill the gap in my knowledge the best I could, as I never got to take a dedicated class about the topic. This inspired me to create a program that would implement some of the basics of machine learning. I created a tool that labeled whether a picture was of a pancake or a waffle. The program achieves around 90% accuracy for the labeling. Due to having a relatively small data set, I used data augmentation to help avoid overfitting. I am still learning about what will make the accuracy better, and ways to prevent overfitting, so this is a work in progress still. Overall, the biggest thing I learned was that having a good dataset for machine learning was just as important as the code and algorithms used.

On the other hand, to help solve my problem that I faced, of gathering a dataset, I used a google image web scraper. The web scraper is able to download nearly all the images of a specified search term automatically by using Selenium. Using this tool allows me to get a decent sized data set of around 700 images, and all I have to do is type in my search term. Most of this I was able to find through a couple github projects, and then combining and modifying them for my use.

Overall, while knowing the difference between a pancake and a waffle is not world changing, I learned a lot, was able to problem solve to find a solution to gathering quick and easy data sets, and created a tool that could classify pancakes and waffles with decently high accuracy.

