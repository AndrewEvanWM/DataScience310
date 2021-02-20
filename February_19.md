1. 
![Alt Text](/convolution1.png) 
![Alt Text](/convolution2.png)
![Alt Text](/convolution3.png)
The first convolution looks at the pixels in the middle edges of the image and removes the importance of the center pixel. This results in a image which is much darker than the other two. The second convolution focuses in on the vertical lines. This convolution diregards the middle column and only focuses on the sides. The final convolution focuses on the horizontal lines. The matrix is all negatives on the top row, 0's in the middle row, and all positives in the bottom row. Functionally, these filters are telling the computer which features of the matrix to focus on. It gives weight to certain pixels and creates an updated image with different features given light. Applying a convolution filter to an image is useful for computer vision because it gives the computer specific patterns to focus. 

2. 
![Alt Text](/pooling.png)
The effect of applying this filter is that the lines seem to be sharpened. This is because the logic behind it is maximizing the values. The pooling loop takes the largest value and applies it to the image matrix. The resulting image is now reduced in size, being half as big as the original image. This method may be useful to find the most important features of an image and make them stand out while not focusing on the less important features. 
