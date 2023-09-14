# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:

## Step1:
Import opencv.

## Step2:
Read the original Image.

## Step3:
Store the required conversion of the image in a variable.

## Step4:
Show the image stored in the given variable.

## Step5:

Destroy all the windows and end the program.

## Program:
```python
# Developed By:  Rama E.K. Lekshmi
# Register Number:212222240082
```
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('ag.jpg')
cv2.imshow('212222240082_Rama E.K. Lekshmi',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# ii)Convert HSV to RGB and BGR
```
import cv2
houseHSVImage = cv2.imread('ag.jpg')
cv2.imshow('212222240082_Rama E.K. Lekshmi',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('ag.jpg')
cv2.imshow('2212222240082_Rama E.K. Lekshmi',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('car.jpg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

# v) Split and merge HSV Image
```
import cv2
image = cv2.imread('ag.jpg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('2212222240082_Rama E.K. Lekshmi',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow


```
## Output:
### i) BGR and RGB to HSV and GRAY
![WhatsApp Image 2023-09-13 at 2 12 39 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/dbbbe319-ae24-4c01-8b13-f1b8923c8e45)
![WhatsApp Image 2023-09-13 at 2 12 51 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/0a9001a3-7de2-4370-8cfd-3534db242a83)


### ii) HSV to RGB and BGR

![WhatsApp Image 2023-09-13 at 3 56 26 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/5f2a7d10-bbfa-42db-8c64-c40f3b1a2548)


### iii) RGB and BGR to YCrCb

![WhatsApp Image 2023-09-13 at 2 15 53 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/e5b110ef-f033-44a1-a109-4d16edaafdde)


### iv) Split and merge RGB Image

![WhatsApp Image 2023-09-13 at 2 14 23 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/7f49e979-1345-4344-8997-6f6fc02ef421)
![WhatsApp Image 2023-09-13 at 2 14 50 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/2a5ada39-0de1-4c91-b514-837fe3be6cba)


### v) Split and merge HSV Image


![WhatsApp Image 2023-09-13 at 4 06 20 PM](https://github.com/Rama-Lekshmi/COLOR-CONVERSION/assets/118541549/de5e5e6a-df49-434c-9d6d-2878536f9aaf)

## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
