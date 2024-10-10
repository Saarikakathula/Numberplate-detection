# Numberplate Detection
### 1. Original image before processing
![Original image before processing](https://github.com/user-attachments/assets/fa3981b9-8513-4580-807e-ff17e48ace16)

### 2. Converts the image from RGB (color) to grayscale, making it easier to detect edges and contours.
![grayscale image](https://github.com/Saarikakathula/Numberplate-detection/blob/main/1..jpg?raw=true)

### 3. Applies a bilateral filter to remove noise while preserving edges, improving contour detection.
![Bilateral Image](https://github.com/Saarikakathula/Numberplate-detection/blob/main/2..jpg?raw=true)

### 4. Uses the Canny edge detector to find the edges in the image.
![Canny Edges](https://github.com/Saarikakathula/Numberplate-detection/blob/main/3..jpg?raw=true)

### 5. Draws all the detected contours on a copy of the original image for visualization.
![All Contours](https://github.com/Saarikakathula/Numberplate-detection/blob/main/4..jpg?raw=true)

### 6. Sorts the contours by area and keeps only the largest 30. Smaller contours are discarded as they are unlikely to be number plates.Displays the top 30 contours.
![Top 30 Contours](https://github.com/Saarikakathula/Numberplate-detection/blob/main/5..jpg?raw=true)

### 7. Loops through the contours, finding ones with 4 corners, which are likely to be a rectangular number plate.
![Final image](https://github.com/Saarikakathula/Numberplate-detection/blob/main/final.jpg?raw=true)

### 8. Cropped number plate images
![Cropped images](https://github.com/Saarikakathula/Numberplate-detection/blob/main/cropped_image_save.jpg?raw=true)
![Cropped images](https://github.com/Saarikakathula/Numberplate-detection/blob/main/ss5.PNG?raw=true)
Once the number plate contour is found, the area is cropped and saved as an image for further processing.Draws the detected number plate contour on the original image for final confirmation.
The cropped number plate image is passed to Tesseract to convert the text on the plate to a string.

### 9. Output
![output](https://github.com/Saarikakathula/Numberplate-detection/blob/main/output.jpg?raw=true)
