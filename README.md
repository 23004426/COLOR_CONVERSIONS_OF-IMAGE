# COLOR_CONVERSIONS_OF-IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.

i) Read, display, and write an image.

ii) Access the rows and columns in an image.

iii) Cut and paste a small portion of the image.

iv)To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg ,
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
### Step6:
Convert BGR and RGB to HSV and GRAY
### Step7:
Convert HSV to RGB and BGR
### Step8:
Convert RGB and BGR to YCrCb
### Step9:
Split and Merge RGB Image
### Step10:
Split and merge HSV Image

##### Program:
### Developed By:
### Register Number: 


## Output:

### i) Read and display the image
### Code :
```
import cv2
image=cv2.imread('jaydeep.jpg',1)
image=cv2.resize(image,(300,400))
cv2.imshow('Jaydeep',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### Output :
![image](https://github.com/23004426/COLOR_CONVERSIONS_OF-IMAGE/assets/144979327/84a33a85-211b-42a5-b3d1-6af4a6e581ec)

<br>
<br>

### ii)Write the image
### Code :
```
import cv2
image=cv2.imread('jaydeep.jpg',0)
cv2.imwrite('new.jpg',image)
```
### Output :
![image](https://github.com/23004426/COLOR_CONVERSIONS_OF-IMAGE/assets/144979327/e2f65be2-737d-48bc-a61e-67f7f945e8d3)

<br>
<br>

### iii)Shape of the Image
### Code :
```
import cv2
image=cv2.imread('jaydeep.jpg',1)
print(image.shape)
```
### Output :
![image](https://github.com/23004426/COLOR_CONVERSIONS_OF-IMAGE/assets/144979327/0f8aee92-16a4-48f3-9160-9e8cea66fd0e)

<br>
<br>

### iv)Access rows and columns
### Code :
```
import random
import cv2
image=cv2.imread('jaydeep.jpg',1)
image=cv2.resize(image,(400,400))
for i in range (150,200):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),
                     random.randint(0,255),
                     random.randint(0,255)] 
cv2.imshow('part image',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### Output :
![image](https://github.com/23004426/COLOR_CONVERSIONS_OF-IMAGE/assets/144979327/ee50aa13-c628-402e-88ed-fbca105e40de)

<br>
<br>

### v)Cut and paste portion of image
### Code :
```
import cv2
image=cv2.imread('jaydeep.jpg',1)
image=cv2.resize(image,(400,400))
tag =image[150:200,110:160]
image[110:160,150:200] = tag
cv2.imshow('partimage1',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### Output :
![image](https://github.com/23004426/COLOR_CONVERSIONS_OF-IMAGE/assets/144979327/d904b55d-59a5-4cf7-9a63-154b50c7fc60)

<br>
<br>

### vi) BGR and RGB to HSV and GRAY
### Code :
```
import cv2
img = cv2.imread('jaydeep.jpg',1)
img = cv2.resize(img,(300,200))
cv2.imshow('Original Image',img)
hsv1 = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsv1)
hsv2 = cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsv2)
gray1 = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',gray1)
gray2 = cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',gray2)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### Output :

<br>
<br>

### vii) HSV to RGB and BGR
### Code :
```

```
### Output :
<br>
<br>

### viii) RGB and BGR to YCrCb
### Code :
```

```
### Output :
<br>
<br>

### ix) Split and merge RGB Image
### Code :
```

```
### Output :
<br>
<br>

### x) Split and merge HSV Image
### Code :
```

```
### Output :
<br>
<br>




## Result:
Thus the images are read, displayed, and written ,and color conversion was performed between RGB, HSV and YCbCr color models successfully using the python program.







