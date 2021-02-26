Convolutions

1: Below are the output matrices of the convolutions. 
Matrix (a, b, c) = [[0, 1, 0], [1, 1, 1], [1, 0, 0]]

[[0 0 0 1 0 0 0]

 [0 0 0 0 1 1 4]
 
 [0 0 1 0 1 6 6]
 
 [0 0 0 2 6 8 5]
 
 [0 2 1 0 1 6 2]
 
 [1 0 0 0 3 2 0]
 
 [2 1 0 0 1 2 0]]
 
 Matrix (d, e, f) = [[1, 1, 1], [1, 1, 0], [0, 0, 1]]
 
 [[0 0 2 0 2 1 0]
 
  [0 0 0 0 0 3 4]
  
  [0 0 0 1 2 5 7]
  
  [3 0 1 0 3 6 7]
  
  [1 0 2 0 3 3 5]
  
  [1 0 0 0 0 5 3]
  
  [2 0 0 0 2 1 1]]


2: The purpose of using a 3x3 filter to convolve acreoss a 2D image matrix is to traverse over an image looking for similiar patterns in the image to the filter. This is used by the computer to better find determined structures.

3: It would be useful to include more than one filter to see the differences between the image when different patterns are looked for. It creates different output matrices each focusing on a different aspect of the image. In the mnist dataset I used three seperate filters as apart of the architecture. 


MSE

1: The mean squared error of the top 10 overpriced data is 5,020.01.

2: The mean squared error of the top 10 underpriced data is 4,118.68.

3: The mean squared error of the most accurate 10 data points is 0.038.

4: The most accurate predictions for me came in the 45th percentile. This meant my data tended towards underestimating the value of the houses. 

5: I believe the baths feature to be the most important in predicting home value. In the most overestimated house there was no bathrooms and it significantly decreased the estimated amount. The most underestimated house was the one with 12 bathrooms. On top of these, the others in the top and bottom 10 had larger numbers of bathrooms than the average houses. The machine did a good job of predicting houses with 2 bathrooms, furthering the idea that bathrooms was the most important factor. 
