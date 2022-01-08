# NumberPlateRecognition-Basic
The goal of this work is to gain skills on conventional Image processing and also leverage the use of EasyOCR package and read text from images.
The workplan is as follows:
1. Take individual images
  Some sample images are shown below, they are read using openCV to the system memory
 

2. Preprocess them: Grayscale conversion and noise removal
3. Edge Detection: Using Canny Edge detector
4. Contours estimation
5. Postprocess the contours: 
  5.1 Grab them, Sort them, return top 10 contours
  5.2 For each contour in check if any of them are forming a 4 points bounded polygon
  5.3 Create a mask of this estimated polygon
 6. Extract text from Image:
 7. Rennder the results
