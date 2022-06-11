# SA-C-GENDER-CLASSIFIER
# Algorithm:

1.Install deepface

2.Import necessary packages

3.Read the image

4.Analyze the gender using deepface

## Program:
```
Program to implement Gender Classification
Developed by   : KAYALVIZHI M
RegisterNumber :  212220230024
```
```python
#install deepface
pip install deepface

#import packages
from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt

#read the image
img=cv2.imread('kim.jpg')
plt.imshow(img[:,:,::-1])
plt.show()
img1=cv2.imread('sejeo.jpg')
plt.imshow(img1[:,:,::-1])
plt.show()

#Analyze gender
result=DeepFace.analyze(img,actions=['gender'])
result1=DeepFace.analyze(img1,actions=['gender'])

#print the gender and emotion
print("Gender : ",result['gender'])
print("Gender : ",result1['gender'])
```
## OUTPUT:

![img](https://user-images.githubusercontent.com/75413726/173192284-cd363b4a-1d71-41e3-8b4d-e7f6ba606470.jpg)

![img1](https://user-images.githubusercontent.com/75413726/173192290-8ac1df63-3961-420a-9564-4a83b7d29682.jpg)


