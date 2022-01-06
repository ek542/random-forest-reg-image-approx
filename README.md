# Image Approximation using Random Forest Regressor

In this project, I use random forest regression to approximate an image (Mona Lisa) by learning a function that takes image coordinates as input and outputs pixel brightness. This project is fun/experimental and the code can be used to approximate any other image as well - like an image of your pet or yourself!  

Since this is an RF model, pre-processing steps are minimal. I experiment with number of trees in the random forest, depth of trees, regularization, as well as top down and bottom up pruning strategies (like tuning the minimum number of samples required to split a node and tuning the minimum number of samples required at a leaf node) to improve model performance and prevent overfitting. I also compare the resulting approximated image with one produced using the k-NN regressor (with k=1) to highlight the difference in blocky-ness of the image. 

Adding more trees to the random forest leads to a more blurred/less defined image because the output is a mean (or some kind of average) of various decision trees. After going through this exercise, I found that there is no correct answer as to which combination og hyperparameters is best for approximating such images, but rather that the decision about hyperparameter values would depend on what one is expecting from the approximated image. 
