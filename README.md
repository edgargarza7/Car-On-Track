# Program an Autonomous Car using Computer Vision and Neural Networks

Learn how to use Computer Vison and Neural Networks to drive your autonomous car around a track. This project requires an AutoAuto Car, which can be purchased [here](https://www.autoauto.ai/).

### Step 1: Clone this Repo onto your AutoAuto Device

Follow [these instructions](./Clone_Repo.md).

### Step 2: Install Tensorflow on your AutoAuto Device

Follow [these instructions](./Install_Tensorflow.md).

### Step 3: Try a pre-trained Neural Network model

This repo has a pre-trained Neural Network model saved in the file name `model_01.hdf5`. It was trained on ~8,000 data points to drive around a track at the AutoAuto headquarters (image below).

<img src="https://autoauto-static-uploads.s3.amazonaws.com/2702760e8fc348b795ac597fa376f0ca.JPG" alt="AutoAuto headquarters Car-on-track" width="200"/>

**Very Important:** One of the key facts about Machine Learning is that is is hard! Why is it hard? Well, one reason is that when you train a machine learning model to do a task (like drive a car around a track), the model will learn only what it can _from the data you provide it_. So, if you provide the car training data to drive around a certain track (like the one in the picture above), then the car will learn how to drive on tracks like _that one_. It will **not** learn how to drive on a _different_ track. Super lame, right? One key to success in machine learning is to have a **great** dataset to train your model. You want to have a dataset that represents _all_ the different things your model might encounter in the real world. Now, there are also some tricks we can do to make our datasets better (we'll discuss those in a later lesson), but for now here is the takeaway: the pre-trained network we provide here might not work on a track _you_ build at home (especially if your track is very different from ours). There is no harm in trying it, just keep this important fact in mind while you do. If this model doesn't work on your track, then we will teach you how to collect training data on your track and train your own machine learning model! Get excited!

