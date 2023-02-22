# Eye_Disease_Detection
Our first customized Deep learning model

Aim:

Given an image we attempt to predict whether a person has either of the diseases or has a normal vision
•	Diabetic Retinopathy
•	Glaucoma
•	Cataract



Inputs Received:

We received close to 4000 retinal images pertaining to the above four categories.
The data was split into training and testing data set in the proportion 60% and 40% respectively
For each of the above two categories there are four folders with the respective image sets.

We have built a custom model and not implemented the transfer learning methodology successfully

What are the important points to keep in mind while building a model?

•	The loaded dataset is rescaled to take values between 0 and 1
•	The target image size was fixed to (150,150) to preserve maximum features
•	Categorical Cross entropy was used for multiclass classification
•	An early stopping with patience parameter =5 was used to prevent waste of training time by monitoring loss value
•	Convolution 2D layer was added to suit the image inputs
•	The final layer is a dense layer with 4 neurons(referring to number of output categories)
•	All layers have an activation function of ‘relu’ while the last layer contains ‘SoftMax’ activation function
