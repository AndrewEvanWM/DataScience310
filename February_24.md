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
