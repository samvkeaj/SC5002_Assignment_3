# SC5002_Assignment_3

Repository Organisation:
Classification and Clustering notebooks are organised separately, due to them being done separately, and each of them being very long.
Final Comparison and Conclusion has a short paragraph comparing the two different models. 
The remaining .pth files and data.pk1 files are available, to help reduce the time taken if the code in the classification and clustering notebooks is to be run. 
data.pk1 contains all the extracted features for the Clustering notebook, and can be used to skip the feature extraction step (by utilising the pickle load function).

Dataset: The dataset consists of 75000 images, of which there are 15000 images of 5 different varieties.

Specifically, the images were of the Arborio, Basmati, Ipsala, Jasmine and Karacadag rice varieties.

These images were collated by a contributor on Kaggle, from a few different papers. The details of this can be found under Rice_Image_Dataset, Rice_Citation_Request.txt.

These images are standardised as individual rice grains against a black background, taken with standardised lighting. This allows for the features of each rice grain to be more accurately captured. 

Visually, rice grains usually contain features such as texture, shape, and color. This allows them to be classified and clustered.

Project: Here, we attempt to use **classification and clustering** to see if each image can be clustered or classified accurately. For clustering, feature extraction using the VGG16 model was performed, and then the dimensionality of data was reduced, and fit to a KMeans model. For classification, a CNN model was trained on and evaluted with the images, with a 80-20 train-test split.


**Steps taken:**

Briefly, the steps taken are as follows:

Vetting of 2 different datasets - 1 other dataset had questionable integrity and was also less interesting to us. <br> 
Superficial check for missing values, by looking for any files that are not labelled with class <br>
Data preprocessing - making directory for ease of working with images <br>
Creating function for model training / feture extraction
Perform train-test split, and calculate performance metrics (accuracy, silhouette score, V-measure) <br>
Conduct k-fold cross validation, and calculate performance metrics <br>
Analysis and discussion of results <br>

**Link to slides:** https://entuedu-my.sharepoint.com/:p:/g/personal/misaki001_e_ntu_edu_sg/EcP2eWEWs-1ClXk1mwyrmx8BJSZXlExkdnn7XdKcBarhQQ?e=1cFcZS 

**Individual Contributions:** (Clearly highlight the contributions of each team member in both the GitHub repository and the video)

Both **Misaki** and **Bryant** were involved in selecting datasets, with each examining 1 dataset before the final dataset was selected for use.
**Misaki** was responsible for all code related to the classification model.
**Bryant** was responsible for all code related to the clustering model.
**Bryant** was responsible for interpreting the relative accuracies of the two different models, as well as discussing practical applications where each model would be more suitable.
**Bryant** and **Misaki** added text cells with explanations, such that the notebook had a smooth logical flow.
**Bryant** was responsible for the overall project management, including the GitHub repository and submission of project.
**Charlene** put together most of the slides and video.
**Bryant and Misaki** edited the slides according to what they would be presenting.
