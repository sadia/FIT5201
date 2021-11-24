# Assessment 1 - Linear Regression

## Score: 93.5/100

In this assessment, you need to answer all the questions about KNN, Linear Regression, Regularization, Logistic Regression, K-fold cross-validation, and other concepts covered in Module 1-3. R studio is recommended to use to complete your assessment. All codes need comments to help markers to understand your idea. If no comment is given, you may have a 10% redundancy on your mark. Please refer to weekly activities as examples for how to write comments. After answering all the questions, please knit your R notebook file to HTML or PDF format. Submit both .rmd file and .html or .pdf file to assessment 1 dropbox via the link on the Assessment page. You can compress your files into a zip file for submission. The total mark of this assessment is 100, which worths 30% of your final result.

## Question 1 - KNN (20/20 marks)
In this question, you are required to implement a KNN classifier to predict the class of cancer clumps. The breast cancer dataset is used in this question. A detailed description of this data set can be found at https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Original%29.

Specifically, you need to:
- Split the data set into a training and a test set with the ratio of 7:3. (1 mark)
- Implement KNN classifiers with different K values (from 1 to 15). (5 marks)
- Investigate the impact of different K values (from 1 to 15) on the model performance (ACC) and the impacts of different distance measurements (Euclidean, Manhattan, Canberra, and Minkowski) on the model performance (ACC). Visualize and discuss your findings. (10 marks)
- Implement the Leave-one-out cross-validation for your KNN classifier with the best K value from the above steps. (4 marks)

## Question 2 - Linear Regression (33/35 marks)
In this question, you need to implement a linear regression model to predict the residuary resistance of sailing yachts. The data set used in this question can be found in ‘yacht_hydrodynamics.csv.’ The data set has 7 features, which are summarized as below.

Variations concern hull geometry coefficients and the Froude number:

- Longitudinal position of the center of buoyancy, adimensional.
- Prismatic coefficient, adimensional.
- Length-displacement ratio, adimensional.
- Beam-draught ratio, adimensional.
- Length-beam ratio, adimensional.
- Froude number, adimensional.

The measured variable is the residuary resistance per unit weight of displacement:
- Residuary resistance per unit weight of displacement, adimensional.

Specifically, you need to:

- Perform data pre-processing, including removing invalid data, transforming the categorical features to numerical features or other operations if necessary. (4 marks)
- Split the data set into a training set and a test set, with the ratio of 8:2. (1 mark)
- Implement stochastic gradient descent to train a linear regression model with your training data. Visualize the parameter updating process, test error (RMSE) in each iteration, and cost convergence process. Please be advised that built-in models in any released R package, like glm, are NOT allowed to use in this question. You can choose your preferred learning rate and determine the best iteration number. (8 marks)
- Evaluate your model by calculating the RMSE, and visualizing the residuals of test data. Please note that an explanation of your residual plot is needed. (5 marks)
- Does your model overfit? Which features do you think are not significant? Please justify your answers. For example, you can analyze the significance of a feature from correlation, variance, etc. (8 marks)
- Use the glmnet library to built two linear regression models with Lasso and Ridge regularization, respectively. In comparison to your model, how well do these two models perform? Do the regularized models automatically filter out the less significant features? What are the differences between these two models? Please justify your answers. (8 marks)

## Question 3 - Logistic Regression (40.5/45 marks)
In this question, you are required to implement a Logistic Regression model to classify whether a person has liver disease or not. Please read the sub-questions below carefully for detailed instructions.

Check out the Blood Transfusion Service Center Data Set at https://archive.ics.uci.edu/ml/datasets/ILPD+%28Indian+Liver+Patient+Dataset%29
- Perform data preprocessing to determine and remove invalid samples. Split the data into a training set and a test set with a ratio of 7:3. (2 marks)
- Develop a Logistic Regression model that uses batch gradient descent for optimization. Visualize the parameter updating process, test accuracy (ACC) in each iteration, and the cost convergence process. Please note that you need to develop your model step-by-step. Built-in models in any released R package, like glm, are NOT allowed to use in this question. (10 marks)
- Investigate the influence of different learning rates on the training process and answer what happened if you apply a too small or a too large learning rate. (5 marks)
- Implement and compare the batch gradient descent and the stochastic gradient descent and discuss your findings (e.g., convergence speed). Visualize the comparison in terms of updating process and the cost convergence process. (6 marks)
- Develop a K-fold (K = 10) cross-validation to evaluate your model in step 3. Please note that you need to write R codes to explicitly show how you perform the K-fold cross-validation. Built-in validation methods are not allowed to use. Different metrics, e.g., ACC, Recall, precision, etc. should be used to evaluate your model. (8 marks)
- Use different values of K (from 5 to N, where N denotes the sample number) and summarize the corresponding changes of your model performances. Visualize and explain the changes. (6 marks)
- How can you modify the cost function to prevent overfitting? Discuss the possibility of adding regularization term(s) and summarize the possible changes in the gradient descent process. (8 marks)
