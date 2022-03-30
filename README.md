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
```python
# Developed By: Sherwin Roger R.D
# Register Number : 212220230046
# To Read,display the image
import cv2
image=cv2.imread("1.jpeg")
cv2.imshow("image",image)
# To write the image
cv2.imwrite("image2",image)
# Find the shape of the Image
print(image.shape)
# To access rows and columns
for i in range(70,90):
  for j in range(110,170):
   image[i][j]=[0,0,0]
# To cut and paste portion of image
image[2000:2700,2000:2700]=image[1000:1700,1000:1700]
```
## Output:

### i) Read and display the image
![image](https://user-images.githubusercontent.com/75235128/160843590-6000c9df-c759-437e-9c8a-0d606b572840.png)

### ii)Write the image
![image](https://user-images.githubusercontent.com/75235128/160843720-189421f0-a935-4a7c-9561-bdfefdc99378.png)

### iii)Shape of the Image
![image](https://user-images.githubusercontent.com/75235128/160843790-27bea203-a853-4487-b7c4-7b2899b22e32.png)

### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/75235128/160843893-d12e504d-7f85-4963-b534-c394aa99ce8e.png)

### v)Cut and paste portion of image
![image](https://user-images.githubusercontent.com/75235128/160844026-af002b94-5e22-422c-addc-a901192e4b45.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.
