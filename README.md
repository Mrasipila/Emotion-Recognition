## Emotion Recognition

# In this notebook we study a dataset of facial images with key points (cf image below). We use it for the task of emotion recognition.
![image](https://github.com/Mrasipila/Emotion-Recognition/assets/30113273/ea3bfc71-2bab-4339-a0c2-664e92b1daca)

- We first create region of interest (ROI) based on the key points around the eye, the nose and the mouth to select only the usefull data of the face
- We then use histogram of oriented gradient (HOG) to get the facial features of the different persons on our dataset
- We Impute our data using K-Neirest Neighbor imputation
- We use Principal Component analysis to reduce the dimension of our dataframe since it contains 6 822 900 elements (9450 * 722) on the training set and 1 012 375 (8099 * 125) element on the test set
- We use RandomForest to try to predict labels of emotions 
