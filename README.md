# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:
### Register Number: 
i) #To Read,display the image
```python3
import cv2
image=cv2.imread("flower.jpeg",1)
cv2.imshow("21222240022_G.Chethankumar",image)
cv2.waitKey(0)
cv2.destroyAllwindows()

```
ii) #To write the image
```python3
import cv2
image=cv2.imread("flower.jpeg",1)
cv2.imwrite("flower.jpeg",image)
cv2.imshow("212222240022_G.ChethanKumar",image)
cv2.waitKey(0)
cv2.destroyAllwindows()
```
iii) #Find the shape of the Image
```python3
import cv2
picture=cv2.imread("flower.jpeg",1)
print(picture.shape)
```
iv) #To access rows and columns

```python3
import random
import cv2
image=cv2.imread("flower.jpeg",1)
for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("21222240022_G.ChethanKumar",image)
cv2.waitKey(0)
cv2.destroyAllwindows()
```
v) #To cut and paste portion of image
```python3
import cv2
img = cv2.imread('tree.jpeg', 1)
tag = img[20:80:, 20:80]
img[90:150, 90:150] = tag
cv2.imshow('212222240022_GChethankumar', img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image



### ii)Write the image
![Screenshot from 2023-08-16 22-08-53](https://github.com/Gchethankumar/READ-AND-WRITE-IMAGE/assets/118348224/cc849e2b-a9e7-4471-a41e-2083a2ee66c3)


### iii)Shape of the Image
![Screenshot from 2023-08-16 22-12-48](https://github.com/Gchethankumar/READ-AND-WRITE-IMAGE/assets/118348224/46addbf9-3989-4c23-80d9-26a60d49bb6c)


### iv)Access rows and columns


### v)Cut and paste portion of image

![Screenshot from 2023-08-22 14-49-14](https://github.com/Gchethankumar/READ-AND-WRITE-IMAGE/assets/118348224/9554b7cd-ddab-4aab-98a7-9b144cc86f73)
## Result:
Thus the images are read, displayed, and written successfully using the python program.
