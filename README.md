# Team Project

## Motivation, specific objective, and success criteria for our machine learning model
Breast cancer is the most prevalent cancer among women, representing 25% of all cancer cases in this population. Early detection is vital for improving survival rates and enabling less invasive treatment options. However, current diagnostic methods rely heavily on manual analysis of biopsy samples by pathologists, a process that is time-consuming and subjective, leading to potential inconsistencies in diagnosis.
Our objective is to develop a predictive tool that can accurately differentiate between normal cells and invasive ductal carcinoma (IDC) cells, a common type of breast cancer. By utilizing a dataset of 277,524 image patches from pathology slides of 162 cancer patients, we aim to create a model that can significantly enhance patient outcomes and healthcare efficiency by automating the diagnostic process.
Our success criteria is to train the model and achieve a model accuracy of at least 85% accuracy. We also plan to implement a pipeline that automates the training, evaluation, and logging to ensure reproducibility and efficiency. 

## Features selection for training machine learning model 
We selected convolutional filters in convolutional neural network (CNN) because convolutional layers can act as feature extractors to identify patterns such as edges, shapes, and even more complex shapes. 
In our project, the model needs to differentiate between normal cells and IDC cells. Convolutional layers allows the learning of hierarchical features, starting from edges to more complex patters such as cell shapes and textures in deeper layers. A CNN model with two convolutional layers and dropout regularization was trained. Hyperparameters include learning rate and batch size. Dropout rates were adjusted to reduce overfitting and the number of epochs was varied to find optimal training duration. 
Finally, model performance was evaluated using accuracy and loss. Validation accuracy reached 86.7%. 

## Preprocessing - missing values or outliers 
To the best of our knowledge, there were no missing images. The labeling information was determined based on the folder in which each image was stored.

## Machine learning alorithm selection 
The use of CNN is ideal for our task as they can efficiently detect and classify different cell types based on learned visual features, as explained above. 

# Validation and hyperparameter tuning 
We tuned the hyperparameters by experimenting with different dropout rates to mitigate overfitting and used maximum percentage of the entire dataset (80%) given our computers' processing capabilities. Additionally, we tested various numbers of training epochs to determine the optimal duration for model training. We aimed to improve the model's generalization performance and robustness by adjusting dropout rates and iterating over different training durations. 

## Dataset splitting 
We used 80% of the entire dataset for model learning and 20% of the dataset to evaluate the final model’s performance. 

## Potential ethical implications and biases with our model
The dataset includes image patches taken from larger cancer images, but not all patches will contain cancer cells. As a result, the model may mistakenly learn to identify and label normal cells as cancer cells if they appear in an image patch that also contains cancer cells. This could lead to the model generating false positives, where normal cells are incorrectly classified as cancerous.
Secondly, this dataset contains images from only 280 patients, which is small compared to the larger number of patients the algorithm will encounter once deployed. This limited dataset size increases the risk of overfitting, which means that the model might learn patterns specific to these patients rather than generalizable features applicable to a broader population. 

## Documentation for future reference 
Documenting machine learning pipeline and model architecture is critical for ensuring reproducibility and providing clarity. Key aspects of the project, including preprocessing, model training, and hyperparameter tuning, were documented either directly in the code or in the README file.

## Link to individual videos
Ihor Kylymchuk: 

Raghvendra Mishra: https://drive.google.com/file/d/11RoL_NOKiAdV3-AzVKE-iRVmA_eLhXTA/view?usp=share_link

Jia xin (Janet) Jiang: https://drive.google.com/file/d/1anTjSK138OFp2uDgmexPOh4iXjU5EYtr/view?usp=drive_link

Parva Thakker: 