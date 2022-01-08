# NumberPlateRecognition-Basic
The goal of this work is to gain skills on conventional Image processing and also leverage the use of EasyOCR package and read text from images.
The workplan is as follows:
1. Take individual images
  Some sample images are shown below, they are read using openCV to the system memory
  
 ![image](https://user-images.githubusercontent.com/61786557/148661196-972831c0-8dd3-48ee-bf8f-6fd5b2ba5400.png) ![image2](https://user-images.githubusercontent.com/61786557/148661200-1255b850-cf7f-47a0-b5bc-de1abd1544bd.jpg)
 ![image6](https://user-images.githubusercontent.com/61786557/148661204-d234e2e0-d1ee-4497-b69e-c309ab37741c.jpg)

2. Preprocess them: Grayscale conversion and noise removal
![image](https://user-images.githubusercontent.com/61786557/148661244-6337feb1-69a5-48a9-8fc7-2436e9d70e7e.png)


4. Edge Detection: Using Canny Edge detector
 ![image](https://user-images.githubusercontent.com/61786557/148661250-99b23e84-d478-464c-9dd7-27e051509ed8.png)

6. Contours estimation
7. Postprocess the contours: 
  5.1 Grab them, Sort them, return top 10 contours
  5.2 For each contour in check if any of them are forming a 4 points bounded polygon
  5.3 Create a mask of this estimated polygon
  ![image](https://user-images.githubusercontent.com/61786557/148661266-2a5d8ed9-8c37-40c2-a7e6-67c524b2a190.png)

  
 6. Extract text from Image:
   ![image](https://user-images.githubusercontent.com/61786557/148661272-2e40d4c7-496c-4e78-bc50-51105d1ba8cb.png)

 8. Rennder the results
 ![image](https://user-images.githubusercontent.com/61786557/148661282-a7556d72-6468-459a-8683-e47412a0e7a9.png)

