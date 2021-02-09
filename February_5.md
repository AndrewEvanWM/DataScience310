1. It is important to split data into testing and training data because that is how we truly know how well the neural network is doing. If we used all the data to train the neural network we would not be able to accurately test the neural network. It would have already seen all the images and would know their classification. 

2. The activation agrument relu sets any result less than 0 to 0 to avoid overreactions from the data. The argument softmax is used in the last layer to select the highest percentage and set that to 1 while the others are set to 0. The reason for the 10 neurons is for each of the clothing classifications. These will be the percentages that the image should be classified under and the softmax is used on. 

3. The optimizer is used in the compile function to update the weights and biases to reduce errors. The loss function is a way for the machine to determine how wrong a prediction is in the training of the data, the error. 

4. a. There are 60,000 training images and each are 28x28. 
   b. The length of the training labels is equal to the number of training images, 60,000.
   c. There are 10,000 testing images and each are 28x28. 
   d. Done in pycharm.
   
5. For the first data point in the testing data set, the np.argmax predicted it would be a 7. This is a good guess as the image is included below. 
![Alt Text](/q5.png)
