INDIAN SPACE RESEARCH ORGANISATION
IPRC-MAHENDRAGIRI
 
INPLANT TRAINING REPORT
(26.06.2023 TO 07.07.2023)
Prepared by
NABOTH DEMETRIUS R
MOHAMED ASLAM K
INPLANT TRAINEE (Data Science)


     Guided By:					          Approved By:			   	     
	

   				
     Anitha T,				        	
     Mahesh Kumar S
     COWAA, MSA		                               GH, MSA      	


7. Dimensionality Reduction
It's a way of reducing the size of the data set by reducing the number of columns that are Features of the data. There are many methods to reduce the dimension some of the important techniques are
●	Principal Component Analysis (PCA)
●	Linear Discriminant Analysis (LDA)
●	Factor Analysis (FA)
●	Reducing dimension by Neural Networks (NN)

7.1 Principal Component Analysis
   Principal components analysis (PCA), is a statistical technique used to analyze and simplify a dataset by transforming it into a new set of variables called principal components. Each principal component is a linear combination of the original variables in such a way that they capture the maximum amount of variance in the data.
The goal of PCA is to reduce the dimensionality of the dataset while retaining as much information as possible. By representing the data in terms of its principal components, which are orthogonal to each other, PCA helps to uncover the underlying structure and patterns in the data.
The first principal component accounts for the largest possible variance in the dataset, followed by the second principal component, and so on. Each subsequent principal component explains a decreasing amount of variance compared to the previous one. Therefore, by selecting a subset of the principal components that explain a significant portion of the variance, one can effectively reduce the dimensionality of the dataset.
Principal components are computed by finding the eigenvectors and eigenvalues of the covariance matrix or correlation matrix of the original dataset. The eigenvectors represent the directions in the feature space along which the data varies the most, while the eigenvalues indicate the amount of variance explained by each eigenvector.
PCA has various applications in data analysis, such as dimensionality reduction, data visualization, noise reduction, and feature extraction. It is widely used in fields like finance, image processing, genetics, and social sciences to uncover meaningful patterns and simplify complex datasets.

7.2 Linear Discriminant Analysis
Linear Discriminant Analysis (LDA) is a statistical technique used for dimensionality reduction and classification tasks. It aims to find a linear combination of features that maximizes the separation between different classes in the data. LDA is commonly used in machine learning and pattern recognition to analyze and classify datasets.
The goal of LDA is to transform the original feature space into a lower-dimensional space while preserving the discriminatory information between different classes. By projecting the data onto a set of orthogonal axes called discriminant axes, LDA seeks to minimize the within-class scatter and maximize the between-class scatter.
Note: Data should have class or target value to perform LDA

7.2.1 PCA VS LDA
●	To perform Principal Component Analysis we don't require data with target values but for LDA data should have target values.
●	Data is reduced through PCA is applied on unsupervised algorithms but for LDA is applied on supervised algorithms.
●	In PCA dimensions are reduced in such a way that maximum variance is covered but in LDA data is separated by maximum linear separation between them.
●	PCA helps to identify the important features but in LDA it improves the performance of classification algorithms.

7.3 Factor Analysis
Factor analysis is a statistical technique used to identify underlying latent variables, known as factors, which explain the patterns of correlation among a set of observed variables. It aims to uncover the underlying structure or dimensions in a dataset by reducing the number of variables and identifying the common factors that contribute to their variation.
The key idea behind factor analysis is that observed variables are not only influenced by specific factors of interest but also by random or error factors. The goal is to separate the systematic variance (explained by the factors) from the random variance (explained by error factors).

7.4 Reducing dimensions using Neural Network
Reducing dimensions using neural networks typically involves employing techniques such as auto encoders or dimensionality reduction layers. Here's a general overview of how dimensionality reduction can be achieved using neural networks.

7.4.1 Auto encoders
Auto encoders are neural networks designed to reconstruct their input data. They consist of an encoder and a decoder. The encoder maps the input data to a lower-dimensional representation, while the decoder reconstructs the original input from this lower-dimensional representation. By training the auto encoder to minimize the reconstruction error, the encoder effectively learns a compressed representation of the input, resulting in dimensionality reduction.

7.4.2 Encoder-Decoder Networks
Another approach involves using encoder-decoder networks, also known as variation auto encoders (VAEs). VAEs add a probabilistic component to auto encoders, which allows them to generate new samples similar to the input data. VAEs can be used for dimensionality reduction by training the encoder to map the input data to a lower-dimensional latent space with specific properties, such as a Gaussian distribution.

7.4.3 Dimension Reducing Layers
 Some neural network architectures, such as the U-Net or the Inception architecture, include built-in dimensionality reduction layers. These layers reduce the spatial dimensions of the input data while preserving relevant features. They are commonly used in tasks such as image segmentation or object detection.

8. Tasks Completed
8.1 TASK 1 - Connectivity log analysis:
Aim:
To analyze status of the ISRO PFMS Web Interface System-Public Financial Management System (IPWS-PFMS) connectivity monitoring system to address (Either success or failure) and visualize them for a given month.

Algorithm:
1)	Load the necessary files.
2)	Split the date into day month year.
3)	Assign each to its respective columns.
4)	Get the IP, status, month, year.
5)	Visualize the count of the required status using a bar chart.
6)	Using a line plot visualize the fluctuations for the complete month.

8.2 TASK 2 - Principal Component Analysis:
Aim:
To perform dimensionality reduction using principal component analysis (PCA) on given engine data set and find the principal components which explains variance of 90%.

Algorithm:
1)	Load the engine data.
2)	Apply standard scaler to the data (Z score).
3)	Find the principal components which explain 90% variance using line plot.
4)	Perform PCA.
5)	Show how the principal components vary when plotted with time.

8.3 TASK 3 - Linear Discriminant Analysis:
Aim:
To perform dimensionality reduction using linear discriminant analysis (LDA) on given engine datasets and infer how the success-failure points vary from each other.

Algorithm:
1)	Load the datasets.
2)	Merge them into single data after specifying the class value for them.
3)	Perform PCA for the merged data excluding the Time and Class columns.
4)	Perform LDA and plot the prediction on test data.
5)	Increase the failure data thrice to avoid biasing and plot.
6)	Perform LDA on actual data without performing PCA and plot.

9. Conclusion:
It is a privilege to be able to attend this in-plant training in ISRO Propulsion Complex. We learnt about the need for data science to be applied in various fields. We learnt how different kinds of data are used to perform different tasks. The outcome of these tasks can be enhanced by using the data more effectively. We also learnt other systems in IPRC like Networking, Databases, Control centers, Servers, Telecom services and a basic outline of Test facilities. We also learnt different techniques to preprocess the data, reduce the dimensions as the data produced from the tests contain a lot of parameters and what techniques has to be applied for different data in order to get valuable insights. We hope that the knowledge we acquired will be used to further develop systems that use data efficiently.






