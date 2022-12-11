# Emotion Detection through Facial Recognition
Hello:wave::smiley: This project is a part of the AAI-521 course in the Applied Artificial Intelligence Program at the University of San Diego (USD).  
-- Project Status: [Completed] 
## Installation
To use this project, first clone the repo on your device using the command below:

git init

git clone https://github.com/hcyrh/Emotion-Detection.git
## Project Intro/Objective
The main purpose of this project is to successfully detect the emotional state of any person in a photo. We originally thought of this idea in hopes to help those with a form of Autism, such as Asperger's Syndrome, to facilitate their ability to depict the emotional state of the individual they're interacting with. The ultimate goal of this project is to create a simple mobile application where one can point to an individual, and it tells you the emotional state of the opponent in real time. 
## Contributors
Rachel Han 

Jennifer Black (jblack1@sandiego.edu)

Jessica Robledo (jessicarobledo@sandiego.edu)
## Methods Used

Computer Vision
## Technologies

Python
## Project Description
This project utilized the FER-2013 dataset, which contains approximately 30,000 facial RGB images of different expressions, and the main labels of it are divided into 7 types: 0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral. However, in our project, we will only detect three emotions for simplicity sake: happy, sad, angry. The data consists of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centered and occupies about the same amount of space in each image. The training set consists of 28,709 examples and the public test set consists of 3,589 examples.

FER uses geometric based technique for expression recognition, which uses facial landmarks to define vectors used in feature extraction. These vectors can be measurements of distances between different parts of the face, facial angles, curvatures, etc. These measurements are then compared to other faces to learn to identify the emotional classes. Another option could have been to use the appearance-based technique, which uses pixel intensities, meaning it can be affected by lighting and is difficult to troubleshoot. The code we used takes advantage of OpenCV’s cascade classifier to detect the faces and the landmarks that are used in defining the vectors. A kernel goes through all parts of an image and scans for faces by passing them through a sequence of simple to complex face classifiers.
## License
See License
## Acknowledgements 
We would like to thank Dr. Roozbeh Sadeghian for an amazing semester!
