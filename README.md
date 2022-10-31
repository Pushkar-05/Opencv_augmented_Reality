# Opencv_augmented_Reality

import cv2

image = cv2.imread('for_watson.png')

alpha = 80 # Contrast control (1.0-3.0)
beta = 90 # Brightness control (0-100)

adjusted = cv2.convertScaleAbs(image, alpha=alpha, beta=beta)

cv2.imshow('original', image)
cv2.imshow('adjusted', adjusted)
cv2.waitKey()
