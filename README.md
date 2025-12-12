# Semantic Segmentation for Autonomous Navigation

This is a personal project I am working on to apply what I've learned in my Deep Learning course.

As an Automation Engineering student, I am interested in how robots perceive their environment. Before a system can make control decisions (like steering or braking), it needs to understand exactly what is in front of it. This project focuses on that "perception" layer.

## The Goal
The objective is simple: to build a model that takes a video of a street and identifies every object in the scene at the pixel level.
Instead of just putting a box around a car, the model should "color" the image:
*   **Road** -> Green
*   **Cars** -> Blue
*   **Pedestrians** -> Red

## Dataset
I am using the **CamVid** dataset found on Kaggle.
It contains images taken from a car dashboard, where every pixel is already labeled.
You can view the dataset here: [Kaggle Link](https://www.kaggle.com/datasets/carlolepelaars/camvid)

## My Approach
I plan to use an architecture called **U-Net**.

In my coursework, I recently studied **Autoencoders** (networks that compress and then reconstruct data). U-Net works on a similar principle:
1.  **Encoder:** Compresses the image to understand *what* is in it.
2.  **Decoder:** Reconstructs the image to locate *where* things are.

This architecture is perfect for semantic segmentation because it preserves the spatial details needed for navigation.
 
## Project Plan
I am currently in the setup phase. Here is my roadmap:

- [ ]**Theory:** Finished course sections on CNNs and Autoencoders.
- [ ]**Data:** Downloaded and inspected the CamVid dataset.
- [ ]**Preprocessing:** Writing scripts to load and resize the images.
- [ ]**Model:** Building the U-Net model in Python using Keras/PyTorch.
- [ ]**Testing:** Running the model on a test video to see the results.

---
*Note: This project is strictly about visual perception and does not involve vehicle control dynamics.*