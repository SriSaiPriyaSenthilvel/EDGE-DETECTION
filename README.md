# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.

## PROGRAM:
```
Developed by: Sri Sai Priya.S
reg number: 212222240103
```
## IMPORT PACKAGES AND LOAD IMAGES
```
import cv2
import matplotlib.pyplot as plt

img=cv2.imread(r'C:\Users\SEC\Pictures\Screenshots\edge.jpg',0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```
## SOBEL EDGE DETECTOR:
# SOBEL X:
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
# SOBEL Y:
```
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.imshow(sobely,cmap='gray')
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
# SOBEL XY:
```
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.imshow(sobelxy,cmap='gray')
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
# LAPLACIAN EDGE DETECTOR:
```
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.imshow(lap,cmap='gray')
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
# CANNY EDGE DETECTOR:
```
canny=cv2.Canny(gray,120,150)
plt.imshow(canny,cmap='gray')
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
### ORIGINAL IMAGE

![318663596-34e33e95-84e8-499f-bb77-acf70b817bc6](https://github.com/SriSaiPriyaSenthilvel/EDGE-DETECTION/assets/119475702/dd59d602-5a90-465b-957c-aa50cfddfa89)

### SOBEL EDGE DETECTOR
# SOBEL X:

![318663808-20579f17-82f9-4ac6-bf38-eeac8bee3a73](https://github.com/SriSaiPriyaSenthilvel/EDGE-DETECTION/assets/119475702/6d9d49ea-2b4c-4e2a-af09-ba939995a5bf)

# SOBEL Y:

![318663957-cd39129d-24fb-4a09-8013-b4069250b20c](https://github.com/SriSaiPriyaSenthilvel/EDGE-DETECTION/assets/119475702/459c9969-1dc7-475d-b1e2-1b2545e19230)

# SOBEL XY:

![318664093-fefa6cd6-d209-4dc9-b57f-016cedeeb354](https://github.com/SriSaiPriyaSenthilvel/EDGE-DETECTION/assets/119475702/5bdd6c68-9ee9-44a5-a236-db74c604efa3)

# LAPLACIAN EDGE DETECTOR

![318664228-503df0ef-d51e-4ab2-bd85-9b33ed866c1c](https://github.com/SriSaiPriyaSenthilvel/EDGE-DETECTION/assets/119475702/ec8fa9fd-7ffb-4585-9066-f1b89729393f)

# CANNY EDGE DETECTOR

![318664381-699c3399-dee0-4a75-a067-8fdcb1829d82](https://github.com/SriSaiPriyaSenthilvel/EDGE-DETECTION/assets/119475702/10caa8dc-bd1b-4846-8811-bf361932ce19)

## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
