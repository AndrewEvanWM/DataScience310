For this project, I chose the country of Nepal. This country is in the heart of the Himalayas, just south of China and north of India. This location will be interesting to study for the various regions in relation to the wealth of the individuals in the DHS study. 

The first model to be used on this dataset is a penalized logistic regression. For this model, there was a split and sample of the data taken. From here, an evaluation of the AUC - ROC values produced can be done. The "top_model" with the largest AUC was 0.0001 with mean area of .603. Included below is an image of the area under the curve as the penalty increases.

![Alt_Text](/lr_plot.png)

As pictured above, there is a steady line at the beginning hovering at the .603 area under the ROC curve mark. There is even a slight peak from a penalty of .000259 to .000329 but each value's mean is still .603. This is why I selected the 6th penalty, .000329. From here a ROC plot was completed on the data, which is pictured below. 

![Alt_Text](/lr_auc.png)

From this image we can see that one wealth outcome stands above the rest in being predicted. The further away from the 45 degree dotted line, or a purely random predictor, the better the predictions. The wealth group 5 is the most accurately predicted. Second is the wealth group 1. The model had a challenging time predicting the middle three wealth groups, which would be expected as they are the most similar to each other and the model likely incorrectly classified between these wealth groups. 

The next model to be interpreted was a random forest. From here the AUC - ROC values for the randomly seleected predictors and the minimal node size were able to be produced. Below is the plot of the results.

![Alt_Text](/rf_res.png)

The next step was to look at the ROC plots. Below are the curves for each of the wealth groups as well as a comparison to the penalized logistic regression.

![Alt_Text](/rf_auc.png)
![Alt_Text](/rf_lr_auc.png)

From the first image, we can see that the predictions of the middle three wealth groups, 2, 3, and 4, have improved slightly. Further there has been an increase in both wealth group 1 and 5. This comparison can best be pictured in the second image above where all the red lines, for the random forest, are above their counterpart for the blue lines, the logistic regression. From this interpretation it can be assumed that the random forest does a better job of classifing the wealth groups than the logistic regression. Next, there can be an examination of the relative importance of each feature to the predictive power of the random forest. Below is a graph which displays the importance of each feature. 

![Alt_Text](/rf_fit.png)

From this image, we can tell that age is the most important predictor of the model, nearly doubling size the second place. The least two important factors are education and gender, with gender being the less important of the two. This suprised me, as I would have expected education to be the most important predictor, but from the data we can see that it is truly age which is the greatest predictor. 

