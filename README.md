# COLOR_CONVERSIONS_OF-IMAGE
## AIM
Write a Python program using OpenCV that performs the following tasks:

i) Read and Display an Image.

ii) Draw Shapes and Add Text.

iii) Image Color Conversion.

iv) Access and Manipulate Image Pixels.

v) Image Resizing

vi) Image Cropping

vii) Image Flipping

viii)	Write and Save the Modified Image


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Load an image from your local directory and display it.
### Step2:
o	Draw a line from the top-left to the bottom-right of the image.
o	Draw a circle at the center of the image.
o	Draw a rectangle around a specific region of interest in the image.
o	Add the text "OpenCV Drawing" at the top-left corner of the image.

### Step3:
o	Convert the image from RGB to HSV and display it.
o	Convert the image from RGB to GRAY and display it.
o	Convert the image from RGB to YCrCb and display it.
o	Convert the HSV image back to RGB and display it.

### Step4:
o	Access and print the value of the pixel at coordinates (100, 100).
o	Modify the color of the pixel at (200, 200) to white.

### Step5:
o	Resize the original image to half its size and display it.
### Step6:
o	Crop a region of interest (ROI) from the image (e.g., a 100x100 pixel area starting at (50, 50)) and display it.
### Step7:
o	Flip the original image horizontally and display it.
o	Flip the original image vertically and display it.

### Step8:
o	Save the final modified image to your local directory.


## Program:
### i)Read and Display an Image
```python
import cv2

# Path to the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Display the image
cv2.imshow('Image', image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
### ii)Draw Shapes and Add Text
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Draw a rectangle
cv2.rectangle(image, (50, 50), (200, 200), (0, 255, 0), 2)

# Draw a circle
cv2.circle(image, (300, 300), 50, (255, 0, 0), 2)

# Add text
cv2.putText(image, 'OpenCV', (100, 400), cv2.FONT_HERSHEY_SIMPLEX, 1, (0, 0, 255), 2)

# Display the modified image
cv2.imshow('Shapes and Text', image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

### iii)Image Color Conversion
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Convert to grayscale
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
cv2.imshow('Grayscale Image', gray_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Convert to HSV
hsv_image = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
cv2.imshow('HSV Image', hsv_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

### iv)Access and Manipulate Image Pixels
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Access pixel at (100, 100)
pixel = image[100, 100]
print(f'Pixel value at (100, 100): {pixel}')

# Modify pixel value
image[100, 100] = [0, 0, 255]  # Set pixel to red

# Display the modified image
cv2.imshow('Modified Pixel Image', image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
### v)Image Resizing
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Resize image to 300x300
resized_image = cv2.resize(image, (300, 300))
cv2.imshow('Resized Image', resized_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

### vi)Image Cropping
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Crop the image
cropped_image = image[50:200, 50:200]
cv2.imshow('Cropped Image', cropped_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

### vii)Image Flipping
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Flip image horizontally
flipped_image = cv2.flip(image, 1)
cv2.imshow('Flipped Image', flipped_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

### viii)Write and Save the Modified Image
```python
import cv2

# Read the image
image_path = r'C:\Users\admin\Downloads\WhatsApp Image 2024-07-02 at 3.28.06 PM.jpeg'
image = cv2.imread(image_path)

# Save the modified image
cv2.imwrite('modified_image.jpg', image)
print('Image saved as modified_image.jpg')
```

### Developed By:Gokkul M
### Register Number: 212223240039

## Output:

### i)Read and Display an Image
![image](https://github.com/user-attachments/assets/b6383364-0f8e-496c-b6ef-aa830b3244d5)

### ii)Draw Shapes and Add Text
![image](https://github.com/user-attachments/assets/2d896b77-ece3-4db7-952b-6ef3b747da7c)

### iii)Image Color Conversion
![image](https://github.com/user-attachments/assets/bfccabae-1af2-41f5-a512-9fe12ae7636b)

### iv)Access and Manipulate Image Pixels
![image](https://github.com/user-attachments/assets/005c5fdc-2dd4-4b64-af87-1339a2134244)

### v)Image Resizing
![image](https://github.com/user-attachments/assets/4e085da6-edff-4026-9b7d-3eb3f3ea001f)

### vi)Image Cropping
![image](https://github.com/user-attachments/assets/85495c6a-83d5-42f2-ae53-b3c497180092)

### vii)Image Flipping
![image](https://github.com/user-attachments/assets/0edff076-ab1d-4070-9ba2-3e3bc3efb019)

### viii)Write and Save the Modified Image
![image](https://github.com/user-attachments/assets/5a3b1bef-81a8-4e47-a428-8133dd7e0d24)

## Result:
Thus the images are read, displayed, and written ,and color conversion was performed  successfully using the python program.







