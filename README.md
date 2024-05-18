import cv2 
import numpy as np 
# Read the image 
img = cv2.imread("shadow.jpg", 1) 
# Define the kernel 
kernel = np.ones((5, 5), dtype="uint8") 
# Perform erosion and dilation 
img_erosion = cv2.erode(img, kernel, iterations=1) 
img_dilation = cv2.dilate(img, kernel, iterations=1) 
# Display the images 
cv2.imshow("Input", img) 
cv2.imshow("Erosion", img_erosion) 
cv2.imshow("Dilation", img_dilation) 
# Wait indefinitely until a key is pressed 
cv2.waitKey(0) 
# Destroy all windows 
cv2.destroyAllWindows() 
