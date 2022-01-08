# NumberPlateRecognition-Basic
The goal of this work is to gain skills on conventional Image processing and also leverage the use of EasyOCR package and read text from images.
The workplan is as follows:
1. Take individual images
  Some sample images are shown below, they are read using openCV to the system memory
  
 ![image](https://user-images.githubusercontent.com/61786557/148661196-972831c0-8dd3-48ee-bf8f-6fd5b2ba5400.png) ![image2](https://user-images.githubusercontent.com/61786557/148661200-1255b850-cf7f-47a0-b5bc-de1abd1544bd.jpg)
 ![image6](https://user-images.githubusercontent.com/61786557/148661204-d234e2e0-d1ee-4497-b69e-c309ab37741c.jpg)

2. Preprocess them: Grayscale conversion and noise removal

![image](https://user-images.githubusercontent.com/61786557/148661333-05e33f86-c26b-4c9d-8195-588d043b761b.png)

![image](https://user-images.githubusercontent.com/61786557/148661244-6337feb1-69a5-48a9-8fc7-2436e9d70e7e.png)

![image](https://user-images.githubusercontent.com/61786557/148661456-8af77628-bf14-46d1-806c-386a7cc59113.png)


3. Edge Detection: Using Canny Edge detector

![image](https://user-images.githubusercontent.com/61786557/148661347-e30156a5-e659-40c2-9aa1-613bad563c91.png)


 ![image](https://user-images.githubusercontent.com/61786557/148661250-99b23e84-d478-464c-9dd7-27e051509ed8.png)
 
 ![image](https://user-images.githubusercontent.com/61786557/148661462-e85fe456-93d9-46e9-83c5-267300d6330d.png)


4. Contours estimation
5. Postprocess the contours: 
  5.1 Grab them, Sort them, return top 10 contours
  5.2 For each contour in check if any of them are forming a 4 points bounded polygon
  5.3 Create a mask of this estimated polygon
  
  ![image](https://user-images.githubusercontent.com/61786557/148661353-1158599a-70a3-409e-b426-2a25a20372f4.png)


  ![image](https://user-images.githubusercontent.com/61786557/148661266-2a5d8ed9-8c37-40c2-a7e6-67c524b2a190.png)
  
  ![image](https://user-images.githubusercontent.com/61786557/148661473-c271833e-3145-40bf-a275-d80b5b3120f9.png)


  
 6. Extract text from Image:
 
   ![image](https://user-images.githubusercontent.com/61786557/148661362-1b176354-c54b-41c6-9d53-7fc0523dbcb9.png)

   ![image](https://user-images.githubusercontent.com/61786557/148661272-2e40d4c7-496c-4e78-bc50-51105d1ba8cb.png)
   
   ![image](https://user-images.githubusercontent.com/61786557/148661483-48acb5a8-7f21-4fea-9468-3c0f24b971ae.png)


 7. Rennder the results
 
 ![image](https://user-images.githubusercontent.com/61786557/148661432-639baef9-a6b1-42f5-8a45-b91f2f641386.png)

 ![image](https://user-images.githubusercontent.com/61786557/148661282-a7556d72-6468-459a-8683-e47412a0e7a9.png)
 
 ![image](https://user-images.githubusercontent.com/61786557/148661506-1ed5e847-bba2-403c-9bf3-b597ae677ba5.png)
 
 Conclusion:
 -This approach being a classical approach works fine with the automobile images having number plates straight withoout distorted, if in case the numberplate is distorted it looses it's accuracy in prediction. 
 - Since we use the contour forming a rectancgle and hard coding it to be the numberplate there is always a chance that it recognizes closed polygons like head lights as a number plate, which was the case in the last image
 -This can either be overcomed by including image wrapping and other image enhancing techniques in the preprocessing steps.
 -One could also use the Machine Learning approaches detecting the numberplates and then extracting text from them.


