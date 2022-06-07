# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.
 
## Program:
```
/*
Developed by   : harish.G
Register Number: 212220230021
*/
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((300,700),dtype='uint8')
font=cv2.FONT_ITALIC=3
img2=cv2.putText(img1,"harish",(5,70),font,3,(255),5,cv2.LINE_AA)
cv2.imshow("Original",img2)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element
kernel=np.ones((5,5),np.uint8)
kernal1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
erode=cv2.erode(img2,kernel)
cv2.imshow("Erosion1",erode)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Dilate the image
dilute=cv2.dilate(img2,kernel1)
cv2.imshow("Dilution",dilute)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### Display the input Image


![zx]![harish 1](https://user-images.githubusercontent.com/75246297/172308839-cf53ad29-5ab4-47a3-a806-7872bb970046.jpg)



### <br><br>Display the Eroded Image
![zx1]![har2](https://user-images.githubusercontent.com/75246297/172308869-f34ab1fd-4d08-46a9-9bb1-71fbf97b3625.jpg)




### Display the Dilated Image
![zx3]![har3](https://user-images.githubusercontent.com/75246297/172308892-b21b5d7f-70be-4d50-bf69-0dbc5a077d1b.jpg)



## <br><br><br><br>Result
Thus the generated text image is eroded and dilated using python and OpenCV.
