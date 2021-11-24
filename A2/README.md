# Assessment 2 - Latent Variables & Neural Networks
In this assessment, you need to answer two questions about EM, clustering, classification, nerual networks, and other concepts covered in Module 4 and 5. R studio is recommended to use to complete your assessment. All codes need comments to help markers to understand your idea. If no comment is given, you may have a 10% redundancy on your mark. Please refer to weekly activities as examples for how to write comments. After answering all the questions, please knit your R notebook file to HTML or PDF format. Submit both .rmd file and .html or .pdf file to assessment 1 dropbox via the link on the Assessment page. You can compress your files into a zip file for submission. The total mark of this assessment is 50, which worth 20% of your final result.

## Score: 17.6/20

### Question 1: EM for Document Clustering [30 Marks]
In this question, you need to develop an EM based document clustering algorithm using both soft and hard approches. Please read Activity 4.1 and 4.2 carefully before answering this question.

- Perform data preprocessing and feature extraction as necessary. [5 marks]
- You need to implement both soft and hard EM-trained GMMs within the given interface and use the Boolean parameter ‘hardclustering’ to decide which GMM is activated. The GMM function interface has been defined, in which function inputs and output are specified. Please don’t rename the function or change its input or output. [10 marks]
- Implement a function that use true labels to evaluate your clustering performance. Please read below instructions for more details. [10 marks]
- Compare the clustering performances of using word count and Term Frequency–Inverse Document Frequency (TFIDF) as features, and explain your results. [5 marks]

### Question 2 Neural Network [20 Marks]
In this question, you are required to construct a neural network classifier with the H2O library. The MINST dataset is used in this question. In consideration of the computation cost, only a portion of the MINST dataset is used, with training (training.xlsx) of 10,000 records and test sets (testing.xlsx) containing 5,000 records, respectively.

Detailed requirements are listed as below.

- Build a 3-layer neural network with only one hidden layer. Change the number of neurons in the hidden layer from 10 to 50 and record the test classification accuracy accordingly. [10 marks]
- Visualize the classification accuracy against the neuron number and explain your findings. [5 marks]
- Try to construct a deeper neural network with more hidden layers to see if there is any improvement on the test classification performance. This is an open question, you can determine the number of hidden layers and the neuron numbers in each hidden layer. Summarize and explain your results. [5 marks]

