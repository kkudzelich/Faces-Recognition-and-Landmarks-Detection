# Facial Recognition and Landmarks Detection

## Project description

__The project:__ An interactive advertising campaign in the mall to increase visitor engagement and increase sales.

__Client:__ An advertiser interested in innovative methods of attracting customers.

__Task:__ Creating a system that identifies loyal customers and adapts advertising content in real time based on their reactions and emotions.

__Decision:__
+ **Face classification model:** Identification of regular customers to offer personalized promotions and discounts.
+ **Keypoints detection model:** Analysis of visitors' reactions to commercials and interactive stands.

__How it works:__
Cameras in the mall identify regular customers and offer them personalized discounts and offers.
Interactive advertising stands track the reactions of visitors and adapt the content depending on their emotions and engagement.
The system offers additional information or discounts when identifying interest in a particular product.
The advertiser receives data on the effectiveness of the campaign to optimize strategies.

## Justification of the approach

+ **Face Recognition**:
I decided to use the Face Classification model __with keypoints as features__. The keypoints of the face are unique patterns that allow you to reliably identify each person and to efficiently extract unique facial characteristics that remain stable under various conditions, such as facial expressions or viewing angles.
<p align="center"> <img src="![landmarks_numbered](https://github.com/kkudzelich/Facial-Classification-and-Landmarks-Detection/assets/107845717/0f2a970b-0b01-4408-b28e-e9e99d1d8e91)" align="middle" alt="drawing" width="300px"> </p>

In addition, the usage of keypoints reduces the dimensionality of the data, which simplifies the process of training the model and increases its performance. Thus, I achieved 93% accuracy in Facial Recognition with both KNN and Feed Forward Neral Network.
<p align="center"> <img src="![image](https://github.com/kkudzelich/Facial-Classification-and-Landmarks-Detection/assets/107845717/8692f85e-a8bf-46c4-aafb-cd219fbc1bec)" align="middle" alt="drawing" width="300px"> </p> 

+ **Facial Landmarks Detection with a **:
This task was solved using Convolutional Neural Network. I tried both a custom one with the selection of different parameters and pretrained ones (ResNet18, EfficientNet, MobileNetV2) __with fune-tuning__ on my data. __MobileNetV2__ turned out to be the best in quality and the fastest.
<p align="center"> <img src="![image](https://github.com/kkudzelich/Facial-Classification-and-Landmarks-Detection/assets/107845717/5065b42b-669b-4eb2-b890-f213112b449a)" align="middle" alt="drawing" width="400px"> </p>
