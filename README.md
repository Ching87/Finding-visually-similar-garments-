# Finding-visually-similar-garments-
 

# Introduction:
Garments in the fashion domain can be of multiple shapes, sizes, and colors. Finding garments similar to each other is an important feature used by e-commerce websites to show recommendations to its users.We would like to find visually similar garments for any input garment from within a given dataset of garment
images.

## Goal: 
Given a database of fashion garment images, the goal is to find 10 visually similar garments from the database, for an given input query garment image.


### Approach:
Here, i have used the pretrained weights of MobileNetV2 architecture in order to extract the salient image features. It is lighter and faster. I have also applied GlobalAverage Pooling on the output layer of the model in order to reduce the output shape. For every image feature, I have calculated the euclidean distance with each other and store the distances in a 2D Numpy array (in the form of a symmetric matrix). The distance matrix is then saved in a compressed .npz file.


### Usage
The fashion industry occupies a significant position in the global economy and involves large industrial chains, including garment design, production, and sales. In fact, in recent years, there has been an expanding demand for clothing all over the world. In fashion e-commerce platforms, product discovery is one of the key components of a good user experience. There are numerous ways using which people find the products they desire. Similar product recommendations is one of the popular modes using which users find products that resonate with their intent. Generally, these recommendations are not personalized to a specific user.


### Viewing the Results
![image](https://user-images.githubusercontent.com/96677288/184533427-c89048c3-bae8-4ace-9d64-a844814bb83a.png)
![image](https://user-images.githubusercontent.com/96677288/184533489-62539331-7016-4fff-9f27-7abd2dd34ed2.png)
![image](https://user-images.githubusercontent.com/96677288/184533528-3812427e-5e73-455a-8414-08465171583a.png)
![image](https://user-images.githubusercontent.com/96677288/184533551-56f6e34c-1fa0-4b49-b347-4ac6f9d60f76.png)
