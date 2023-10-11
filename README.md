# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.


### Step2:
Create the Text using cv2.putText

### Step3:

Create the structuring element
### Step4:
Use Opening operation.

### Step5:

Use Closing Operation
 
## Program:
#### DEVELOPED BY : JEEVITHA E
### REGISTER NO: 212222230054


# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```


# Create the Text using cv2.putText
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'jeevitha E',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```


# Create the structuring element
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```


# Use Opening operation
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```




# Use Closing Operation
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()
```




## Output:

### Display the input Image

![image](https://github.com/Jeevithaelumalai/OPENING--CLOSING/assets/118708245/aba20780-b36d-47d2-b9f0-5a106025b5e8)


### Display the result of Opening
![image](https://github.com/Jeevithaelumalai/OPENING--CLOSING/assets/118708245/f60b352c-c33c-47ee-9c96-b2e5d5e3a9db)


### Display the result of Closing
![image](https://github.com/Jeevithaelumalai/OPENING--CLOSING/assets/118708245/c65aad9d-4437-4854-b3aa-498cc8527506)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
