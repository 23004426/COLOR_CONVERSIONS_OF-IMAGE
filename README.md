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

```
### Output :
<br>
<br>

### iv)Access rows and columns
### Code :
```

```
### Output :
<br>
<br>

### v)Cut and paste portion of image
### Code :
```

```
### Output :
<br>
<br>

### vi) BGR and RGB to HSV and GRAY
### Code :
```

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







