# NumberPlateRecognition-Basic
The goal of this work is to gain skills on conventional Image processing and also leverage the use of EasyOCR package and read text from images.
The workplan is as follows:
1. Take individual images
  Some sample images are shown below, they are read using openCV to the system memory
 ![image](https://user-images.githubusercontent.com/61786557/148661196-972831c0-8dd3-48ee-bf8f-6fd5b2ba5400.png) ![image2](https://user-images.githubusercontent.com/61786557/148661200-1255b850-cf7f-47a0-b5bc-de1abd1544bd.jpg)
 ![image6](https://user-images.githubusercontent.com/61786557/148661204-d234e2e0-d1ee-4497-b69e-c309ab37741c.jpg)



2. Preprocess them: Grayscale conversion and noise removal
3. Edge Detection: Using Canny Edge detector
4. Contours estimation
5. Postprocess the contours: 
  5.1 Grab them, Sort them, return top 10 contours
  5.2 For each contour in check if any of them are forming a 4 points bounded polygon
  5.3 Create a mask of this estimated polygon
 6. Extract text from Image:
 7. Rennder the results
