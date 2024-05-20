# deep-learning-challenge

This repo houses a number of files that contain code that builds a deep learning model aimed at predicting if a charity application will be approved. Both ipynb and h5 versions of the files exist so that they can be worked with in multiple environments. The AplhabetSoupCharity files contain the original process of building the model, while the AplhabetSoupCharity_Optimization files contain tweaks to the model in an attempt to improve results. The results of the work are highlighted below, and can also be found in the report-template.md file.

***Overview***

The purpose of this analysis was to develop a deep learning model to predict whether a charity application will be successful based on various features provided in the dataset. The primary objective was to achieve a model accuracy of at least 75%.

***Results***

***Data Preprocessing***

Target Variable(s)
   - IS_SUCCESSFUL: This variable indicates whether a charity application was successful (1) or not (0).

Feature Variable(s)
   - APPLICATION_TYPE
   - AFFILIATION
   - CLASSIFICATION
   - USE_CASE
   - ORGANIZATION
   - STATUS
   - INCOME_AMT
   - SPECIAL_CONSIDERATIONS
   - ASK_AMT

Variables Removed
   - EIN
   - NAME
   - These variables were removed as they are identifiers and do not contribute to the prediction.

***Compiling, Training, and Evaluating the Model***

Model Architecture
   - Neurons:
     - First Hidden Layer: 256 neurons
     - Second Hidden Layer: 128 neurons
     - Third Hidden Layer: 64 neurons
   - Layers:
     - Input Layer
     - Three Hidden Layers
     - Dropout Layer
     - Output Layer
   - Activation Functions:
     - ReLU for hidden layers
     - Sigmoid for output layer

   The choice of neurons and layers was to capture complex patterns in the data, with dropout to prevent overfitting.

***Model Performance***
   - Achieved Accuracy: 72.54%
   - Target Accuracy: 75%
   - Despite various adjustments, the target accuracy was not achieved.

***Steps Taken to Increase Performance***
   - Adjusted the number of neurons and layers
   - Implemented dropout regularization
   - Used L2 regularization
   - Tweaked the learning rate
   - Increased the batch size
   - Implemented early stopping to prevent overfitting

***Summary***

The deep learning model achieved an accuracy of 72.54%, which was below the target of 75%. Various techniques were employed to enhance the model's performance, including adjustments in architecture, regularization, and hyperparameters. However, these efforts resulted in only marginal improvements.

***Recommendation***

To potentially solve this classification problem more effectively, exploring other machine learning models such as Random Forests, or even more sophisticated deep learning architectures e.g. Convolutional Neural Networks, could be beneficial. Models such as Random Forests, in particular, are known for their robustness and ability to improve predictive performance by combining the strengths of multiple models. This approach could help achieve the desired accuracy target and provide more reliable predictions.
