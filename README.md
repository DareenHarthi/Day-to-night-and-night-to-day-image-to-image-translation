# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Data Science: Capstone Project

## Day to night and night to day image to image translation

<img src = "https://astroedu.iau.org/media/cache/b7/11/b71141fd0e9652619b4cbdab73687697.jpg">

## Problem Statement
Many image processing project that uses images of places or roads takes to long to Collect images because conditions such as weather and lighting can change considerably and they need to take all cases to get good results, to solve this problem and speed the process of collecting images I used Generative Adversarial Networks (GANs) to generate images with different weather conditions, also convert day images to night and vice versa.
   - **Potential Audience**<br> 
   Any one who needs an image generator with different weather conditions.
   - **Goals**<br> 
   Generate images with different weather conditions.
   - **Success Metrics**<br> 
   The result of test data, if the model generates correct images with appropriate weather filters, also Generator loss function should approach to zero.

## Dataset and  Data 

In this project I have to datasets of images, daylight images from Udacity and night images which are frames of Youtube video "Night driving front view", the number of images in the tow dataset is 33149 frame, train size is 21799 frame and test size 11350 frame.

## EDA and Preliminary Analysis
Since the datasets are frames the images will be duplicated, Therefore each 2 second or 60 frames I took 1 frame, Hence the train size becomes 500 images, and the test size becomes 53 images.

## Model
In this project I used CycleGAN to perform style transfer from day to night and night to day.
