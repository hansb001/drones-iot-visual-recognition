# Drones-IoT-Visual-Recognition
Save Lives with Drones / IoT / Visual Recognition - Call for Code Hands on Lab

## Introduction

This hands on lab uses drone aerial images, Watson Studio and Watson Visual Recognition to survey wildfire damaged neighborhoods and identify burned homes and intact homes.

![Watson Studio screenshot](screenshots/WatsonStudio-VisualRecognitionModelTestResults.png)

## Learning objectives

After completing this tutorial you will be able to:

* Create a Visual Recognition model in Watson Studio running in IBM Cloud
* Capture images from a drone and zip them into a class
* Train a model to identify objects in the images
* Score and count the identified objects

## Prerequisites

This tutorial can be completed using an IBM Cloud Lite account.

* Create an [IBM Cloud account](https://ibm.biz/Bdq2LV)
* Log into [IBM Cloud](https://console.bluemix.net/login)

## Estimated time

You can complete this task in no more than 45 minutes.

# Hands on Lab Overview

The outline below provides a high level overview of the steps included in the lab instructions.  

## Step 1 - Learn about Drones

There are many types of drones available that range from toys to industrial use cases.  Many of the drones now include a camera that can store or stream aerial video to the ground. Using the livestream video frames, we can sample frames and send the images to Watson Visual Recognition for classification.
- Pocket toy drones
  - [Contixo F17](https://www.contixo.com/f17-quadcopter-4k-hd-drone)
- Tello - Control a [Tello Drone using Node-RED](https://github.com/johnwalicki/Node-RED-Tello-Control)
- Hobbyist drones
- Commercial drones

For this lab, we are not flying the drone indoors or venturing out into a field.  If you are interested in purchasing a drone, the instructor(s) can share some of their drone experiences and recommendations.

## Step 2 - Capturing Images

One of the fun experiences of flying a drone is capturing video or pictures from a unique aerial perspective. You can use your drone to capture images of interesting objects that you want to train a visual recognition model to autonomously identify.

In this lab, we have created three zip files of pictures recorded by drones. The lab will use these images to identify neighborhoods affected by the devastating 2018 West Coast wildfires. These images will be used as our training set.
- Aerial drone images of burned homes - [BurnedHomes.zip](classes/BurnedHomes.zip)
- Aerial drone images of intact homes - [AerialHomes.zip](classes/AerialHomes.zip)
- Aerial drone images of forests, roads, rivers to be used for the negative class. [NotHomes.zip](classes/NotHomes.zip)

*Source attribution: USA Today [article](https://www.usatoday.com/in-depth/news/nation-now/2018/08/02/drone-aerials-california-wildfire-devastation/889885002/), various internet sources*


## Step 3 - Watson Studio
In this section, we will create a Watson Studio instance, create a Project and Watson Visual Recognition model to identify images in several classes.

- Create a Watson Studio instance - follow these [instructions](STUDIO.md)
- Create a Project
- Create a Visual Recognition model - follow these [instructions](VISRECO.md)
- Upload three zips to Cloud Storage
- Create a class *Burned Home* 
- Create another class *Intact Home* 
- Create a negative class using the *Not Homes* images 
- Train your model - wait a few minutes

## Step 4 - Test your model
In this section you will use sample images to confirm your model.
- Test your model - follow these [instructions](VRMTEST.md)

## Step 5 - Implement this model in your Application

- Embed your model into an application using these code snippets

Let's get started - [Set up Watson Studio](STUDIO.md)

*Quick links :*
[Home](/README.md) - [**WildFires**](WILDFIRES.md) - [Watson Studio](STUDIO.md) - [Visual Recognition Model](VISRECO.md) - [Test and Deploy](VRMTEST.md)
