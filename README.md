# Finding-visually-similar-garments-
 

# Introduction:
Garments in the fashion domain can be of multiple shapes, sizes, and colors. Finding garments similar to each other is an important feature used by      e-commerce websites to show recommendations to its users.We would like to find visually similar garments for any input garment from within a given dataset of garment
images.

## Goal: 
Given a database of fashion garment images, the goal is to find 10 visually similar garments from the database, for an given input query garment image.


### Approach:
Here, i have used the pretrained weights of MobileNetV2 architecture in order to extract the salient image features. It is lighter and faster. I have also applied GlobalAverage Pooling on the output layer of the model in order to reduce the output shape to 
