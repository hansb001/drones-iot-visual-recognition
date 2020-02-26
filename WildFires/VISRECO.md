*Quick links :*
[Home](/README.md) - [WildFires](WILDFIRES.md) - [Watson Studio](STUDIO.md) - [**Visual Recognition Model**](VISRECO.md) - [Test and Deploy](VRMTEST.md)
***

## Lab Objectives

In this lab you will create a Visual Recognition model in a Watson Studio Project.  You will learn:

- How to work within a new Watson Studio Project
- How to create a Visual Recognition model

### Watson Studio Projects

Projects are your workspace to organize your resources, such as assets like data, collaborators, and analytic tools like notebooks and models.
The first step is to add Assets to your Watson Studio Project



#### Add Visual Recognition Model
Next step is to add a visual recognition model to the project.

- Click on **Add to project**, a list of assets will appear.
- Choose **Visual Recognition model**
- In the **custom Models** section, choose **Clasify Images** by clicking on **Create model**
- The **Default Custom Model** name is not descriptive so let's rename it
- Click on the **pencil** icon to edit the name
- Rename the model to **Count Burned Homes**



#### Add Custom Classes to the Watson Visual Recognition Model

#### Upload Zip Files to Watson Studio Project
- Three zip files have been prepared which contain aerial drone images
- If you following these steps on the web, download the aerial drone zip files here:
  - [BurnedHomes.zip](classes/BurnedHomes.zip)
  - [AerialHomes.zip](classes/AerialHomes.zip)
  - [NotHomes.zip](classes/NotHomes.zip)
- Click on the **Browse** button
- An operating system native File Dialog will open
- Multi-select the three zip files **BurnedHomes.zip**, **AerialHomes.zip**, **NotHomes.zip**
- Upload these zip files to your Watson Studio project
- You will see the zip files added to the classes section.
- Rename **BurnedHomes.zip** to **Burned Homes**
- Rename **AerialHomes.zip** to **Intact Homes**
- Now add the images from **NotHomes.zip** to the negative class by clicking on **NotHomes.zip**
then select all images and click on **Reclassify** and select the **Negative** class
- Delete the **NotHomes.zip** class

#### Train your Watson Visual Recognition Custom Classifier
- Click on the **Train Model** button
- Wait a few minutes for the model to train on the images

![Watson Studio  screenshot](screenshots/WatsonStudio-VisualRecognitionModelTrain.png)

![Watson Studio  screenshot](screenshots/WatsonStudio-VisualRecognitionModelTraining.png)

#### Congratulations
- Once the model has been trained, click on the **Click here** link to view and test your model.

![Watson Studio  screenshot](screenshots/WatsonStudio-VisualRecognitionModelTrained.png)

#### Review and Test
- Review the Classes and Model details
- Click on the **Test** tab

![Watson Studio  screenshot](screenshots/WatsonStudio-VisualRecognitionModelSummary.png)

Test your model in the next [step](VRMTEST.md)

*Quick links :*
[Home](/README.md) - [WildFires](WILDFIRES.md) - [Watson Studio](STUDIO.md) - [**Visual Recognition Model**](VISRECO.md) - [Test and Deploy](VRMTEST.md)
