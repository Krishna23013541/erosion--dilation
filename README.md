# Exp-9- Record-IMPLEMENTATION OF EROSION AND DILATION
# Reg.No:212223230107
# Name: KRISHNA KUMAR R
# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
### Algorithm:
#### Step1:<br>
Import the necessary pacakages

#### Step2:<br>
Create the text using cv2.putText

#### Step3:<br>
Create the structuring element

#### Step4:<br>
Erode the image


#### Step5: <br>
Dilate the Image

 
## Program:

# Import the necessary packages
````
import cv2
import numpy as np
import matplotlib.pyplot as plt
````

# Create the Text using cv2.putText
````
def load_img():
    blank_img=np.zeros((600,600))
    font=cv2.FONT_HERSHEY_SIMPLEX
    cv2.putText(blank_img,"MANI KUMAR",(50,300),fontFace=font,fontScale=5,color=[255,255,255],thickness=25,lineType=cv2.LINE_AA)
    return blank_img
````


# Create the structuring element
````
image = load_img()
plt.imshow(image, cmap='gray')
plt.show()
````

# Erode the image
````
kernel=np.ones((5,5),np.uint8)
kernel
ersion=cv2.erode(image,kernel,iterations=4)
plt.imshow(ersion,cmap='gray')
````

# Dilate the image
````
dilution=cv2.dilate(image,kernel,iterations=4)
plt.imshow(dilution,cmap='gray')
````



## Output:

### Display the input Image

<img width="512" height="500" alt="image" src="https://github.com/user-attachments/assets/ee8d45bd-4ca1-4d99-b723-f17a6470b471" />



### Display the Eroded Image

<img width="493" height="508" alt="image" src="https://github.com/user-attachments/assets/51fd3df1-ca53-4f5c-9e9e-3e493872e937" />


### Display the Dilated Image

<img width="519" height="507" alt="image" src="https://github.com/user-attachments/assets/7d5ba190-2829-47f4-8f2e-479c4874efae" />


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
