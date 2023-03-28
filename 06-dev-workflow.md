### Development Workflow for AI Systems

This section aims to define a high-level process flow to develop a (standalone) AI-based system from scratch. The steps listed are general and may vary from context to context.

1. Problem Definition: As with all, the journey of AI-based systems also begins with problem definition. A few questions are important to identify if AI is the suitable approach for the problem under consideration. For example, why can't the system be implemented using legacy exhaustive algorithmic approaches? is the system supposed to learn and evolve? Once the need for AI is well understood, the next set of questions arises that tend to define the business objective, target audience, data availability, overall feasibility, and success criteria. Having defined the problem, the next step is to determine if AI/ML can be used to address it.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227782937-6f75873b-61f6-41d6-91f7-39170bbb73c0.png" width="450" height="295" />
</p>

2. Choosing Method: Once the problem is defined and it is decided that it is more viable and suitable to solve it using AI instead of legacy exhaustive methods, the next step is to decide the type of AI to solve the problem. From rule-based AI to different types of ML and deep learning models may be considered and chosen based on the relevant factor. These factors may include the type of problem (e.g., classification, regression, clustering, etc.), type and size of data as the data may be labeled or unlabelled, structured or unstructured, stored using conventional or modern scalable systems, etc.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227783618-8b980958-b6e3-4efa-bc81-62106a0c5343.png" width="450" height="295" />
</p>

3. Data Collection: Having chosen the right methods, the next important step in most cases is sourcing the data. Data may come from the ongoing processes (which makes this step easier) or may base on designed collection (which is usually challenging). Without the right quality and quantity of data, most AI/ML systems cannot be realized. However, some simpler systems might rely on rule-based AI and may not need data as a primary factor to learn from. In other situations, for example, reinforcement learning may also need less prior data to start functioning. Here are some factors related to data collection that are important to consider:
    1. Data Relevance: The data used to train the machine learning model should be relevant to the problem at hand. Irrelevant data can lead to biased or inaccurate predictions.
    2. Data Quantity: The amount of data available for training the machine learning model is a critical factor in determining its performance. Generally, more data leads to better model performance, but too much data can lead to computational and storage issues.
    3. Data Quality: The quality of the data used to train the machine learning model is essential. Poor quality data can lead to inaccurate predictions and models that are not fit for purpose.
    4. Data Bias: The data used to train the machine learning model should be free from any bias. Biased data can result in models that are not equitable or inclusive.
    5. Data Collection Methods: The methods used to collect data can impact the quality and relevance of the data. It is essential to choose appropriate data collection methods that align with the problem at hand.
    6. Data Privacy and Security: Data used in machine learning models may contain sensitive information, and it is essential to ensure that the data collection process is compliant with privacy and security regulations.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227787527-38fc8761-1aa1-4021-bf02-925af5fd8c23.png" width="650" height="215" />
</p>

4. Data Preprocessing: It is usually required to clean, transform and normalize the data to ensure it is in a suitable format for modeling. Depending on the condition of the data, the effort for data preprocessing may vary. Following are some factors related to data preprocessing that are important to consider:
    1. Data Cleaning: The process of identifying and correcting or removing errors, incomplete data, or outliers that can affect the quality of the data.
    2. Data Transformation: The process of converting the raw data into a format that can be used by the machine learning model. This includes converting categorical data into numerical data, scaling or normalizing the data, and performing feature engineering.
    3. Handling Missing Data: The process of identifying and handling missing data in the dataset. This can include imputing missing data, removing rows with missing data, or using models that can handle missing data.
    4. Data Augmentation: The goal of data augmentation is to increase the size and variability of the training dataset by creating additional examples based on the original data. This can be done in a variety of ways, such as by rotating, flipping, or cropping images, or by adding noise or distortions to numerical data.
    5. Data Integration: The process of combining data from different sources or formats into a single dataset that can be used to train the machine learning model.
    6. Data Encoding: The process of converting categorical variables into numerical variables that can be used by the machine learning model. This includes one-hot encoding, label encoding, and ordinal encoding.
    7. Data Balancing: The process of balancing the dataset if it is imbalanced across different outcomes of interest. Imbalanced datasets can negatively impact the performance of the machine-learning model.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227791964-6c5d6863-8d33-493b-94cb-9e87a88f7da2.png" width="720" height="215" />
</p>
      
5. Exploratory Data Analysis: Exploratory Data Analysis (EDA) is an essential step in the machine learning development workflow that involves understanding the data and identifying patterns, relationships, and anomalies. Here are some factors related to EDA that are important to consider:
    1. Data Distribution: The distribution of the data can impact the choice of machine learning algorithm and the interpretation of the results. EDA helps in understanding the data distribution, such as whether it is normally distributed, skewed, or has outliers.
    2. Correlation Analysis: Correlation analysis helps in understanding the relationship between different variables in the dataset. It helps in identifying the most important features and removing redundant features.
    3. Data Visualization: Data visualization techniques, such as scatter plots, histograms, and box plots, help in identifying patterns and relationships in the data. This is important in identifying outliers, understanding the data distribution, and identifying relationships between variables.
    4. Feature Importance: EDA helps in identifying the most important features in the dataset. This helps in feature selection and building a more accurate machine-learning model.
    5. Data Scaling: EDA can help in identifying the scale of the data, such as whether it needs to be normalized or standardized before training the model.
    6. Domain Knowledge: EDA can help in understanding the problem domain and the relevance of different features. This can lead to better feature engineering and model performance.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227792501-fb0ef557-f5e7-4a3b-8db3-e0673c1883b0.png" width="650" height="215" />
</p>

6. Feature Engineering: Feature engineering is a crucial step in the machine learning development workflow that involves selecting and transforming the raw data into meaningful features that can be used to train the machine learning model. Here are some factors and methods related to feature engineering that are important to consider:
    1. Domain Knowledge: Having domain knowledge about the problem and the data can help in identifying relevant features that can contribute to the accuracy of the machine learning model.
    2. Feature Extraction: Feature extraction involves transforming the raw data into a set of meaningful features. This can include techniques such as Principal Component Analysis (PCA), Independent Component Analysis (ICA), and Fourier Transform.
    3. Feature Selection: Feature selection involves selecting the most relevant features that can contribute to the accuracy of the machine learning model. This can be done using techniques such as Correlation-based Feature Selection (CFS), Wrapper-based Feature Selection, and Embedded Feature Selection.
    4. Feature Scaling: Feature scaling involves normalizing or standardizing the features to ensure that they have a similar scale. This is important for algorithms such as K-Nearest Neighbors and Support Vector Machines.
    5. Feature Encoding: Feature encoding involves converting categorical variables into numerical variables that can be used by the machine learning model. This can include techniques such as One-Hot Encoding, Label Encoding, and Binary Encoding.
    6. Feature Combination: Feature combination involves combining multiple features to create new features that can be more informative than individual features. This can include techniques such as Polynomial Features and Feature Interactions.
    7. Feature Generation: Feature generation involves creating new features from existing features using domain-specific knowledge or machine learning algorithms. This can include techniques such as Clustering, Text Analysis, and Image Processing.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227792500-642b223f-4964-4a6b-804e-0e1a12ff9927.png" width="720" height="215" />
</p>

7. Model Selection: Choosing the appropriate AI/ML algorithm for the problem at hand is the next obvious step. While choosing the model, it is important to take into account factors such as the size and type of data, computational resources, and the desired outcome. It is pertinent to mention that the model selection at this stage is from within the category of method decided during step 2. Here are some factors related to model selection that are important to consider:
    1. Problem Type: The type of problem being solved can impact the choice of the machine learning algorithm. For example, classification problems may require different algorithms than regression problems.
    2. Size of the Dataset: The size of the dataset can impact the choice of the machine learning algorithm. Some algorithms may work better with large datasets, while others may be better suited for smaller datasets.
    3. Computational Resources: The volume of computational resources available can impact the choice of the machine learning algorithm. Some algorithms may require more resources, such as memory or processing power, than others.
    4. Accuracy Requirements: The required level of accuracy can impact the choice of the machine learning algorithm. Some algorithms may be more accurate than others, but may also be more complex or require more computational resources.
    5. Interpretability Requirements: The required level of interpretability can impact the choice of the machine learning algorithm. Some algorithms may provide more interpretability than others, making it easier to understand how the model is making its predictions.
    6. Ensemble Methods: Ensemble methods involve combining multiple machine learning algorithms to create a more accurate and robust model. The choice of ensemble method can impact the performance of the model.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227793999-12b64882-089e-40ca-8c59-a0c4d33a236e.png" width="650" height="215" />
</p>
          
8. Model Training and Validation: The chosen model(s) is trained on the preprocessed data and its performance is evaluated using appropriate metrics. Several different models can be trained to select the most suitable one considering the accuracy and efficiency requirements. During validation, the model undergoes a test as if it is deployed in a real environment. Factors like overfitting are preempted and taken care of at this step. Here are some factors and methods related to model training and validation that are important to consider:
    1. Dataset Splitting: The dataset should be split into a training set and a validation set. The training set is used to train the machine learning model, while the validation set is used to evaluate its performance. The typical split is 80% for training and 20% for validation.
    2. Cross-Validation: Cross-validation is a technique that involves splitting the dataset into multiple subsets, training the model on some subsets, and evaluating its performance on others. This can help to reduce the risk of overfitting and provide a more accurate estimate of the model's performance.
    3. Loss Function: The loss function is used to measure how well the machine learning model is performing on the training data. Different machine learning algorithms require different types of loss functions.
    4. Optimization Algorithm: The optimization algorithm is used to adjust the parameters of the machine learning model to minimize the loss function. Different optimization algorithms may work better for different types of machine learning algorithms.
    5. Regularization: Regularization is a technique that is used to prevent overfitting by adding a penalty term to the loss function. Regularization can take different forms, such as L1 or L2 regularization.
    6. Hyperparameter Tuning: Hyperparameter tuning involves selecting the best values for the hyperparameters of the machine learning algorithm. This can be done using techniques such as grid search, random search, or Bayesian optimization.
    7. Performance Metrics: Performance metrics are used to evaluate the performance of the machine learning model. Different performance metrics may be used depending on the problem type, such as accuracy, precision, recall, F1 score, or ROC-AUC score.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227794090-1dc6b5fb-7b27-444b-8fde-ab6d0e4cf4a2.png" width="720" height="215" />
</p>

9. Model Deployment: The system is considered in a ready state after the training and validation cycle is completed. However, the journey does not end here. Most often, the trained models are deployed for use as interactive applications on cloud platforms that need relevant skills. Provision of resources and scaling according to the number of users and access frequency is vital in this context. Here are some factors and methods related to model deployment that are important to consider:
    1. Hardware and Software Infrastructure: The machine learning model requires hardware and software infrastructure to run in a production environment. The infrastructure should be selected based on the specific requirements of the model, such as processing power, memory, and storage.
    2. Data Pipeline: The machine learning model requires a data pipeline to receive input data and produce output data. The data pipeline should be designed to handle the specific data format and volume required by the model.
    3. Model Format: The machine learning model needs to be converted into a format that can be easily loaded and used by the production environment. Common model formats include ONNX, TensorFlow, and PyTorch.
    4. API Design: The machine learning model should be exposed through an API that allows it to be easily integrated into other systems. The API should be designed to handle the specific input and output formats required by the model.
    5. Scalability: The machine learning model should be designed to scale to handle increasing amounts of data and traffic. This may require additional hardware resources or the use of distributed computing technologies.
    6. Security: The machine learning model should be secured to prevent unauthorized access or tampering. This may require the use of encryption, authentication, and access control mechanisms.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227794178-b0659dab-3deb-43b6-8690-1c9bd7f3d039.png" width="650" height="215" />
</p>

10. Monitoring and Maintenance: While the system is in production, continuous monitoring of the performance of the deployed model and making updates as necessary to ensure it remains accurate and relevant is key to a successful system. The data, methods, and models may all need fine-tuning and/or replacements over time as the system evolves. Here are some factors and methods related to monitoring and maintenance that are important to consider:
    1. Data Drift: Data drift refers to changes in the distribution of input data over time. Monitoring for data drift is important to ensure that the deployed machine learning model continues to perform well on new data. This can be done by comparing the distribution of new data to the distribution of the training data.
    2. Model Performance: Monitoring for changes in model performance is important to detect issues such as overfitting or underfitting. This can be done by regularly evaluating the model's performance on a validation set or through other metrics such as precision, recall, and F1 score.
    3. Dependencies: The dependencies of the deployed machine learning model should be regularly updated to ensure that it remains compatible with other software and hardware components. This may involve updating the versions of programming languages, libraries, or operating systems.
    4. Retraining: The deployed machine learning model may need to be retrained periodically to account for changes in the input data or to improve its performance. This may involve collecting new data, selecting a new algorithm or adjusting the hyperparameters, and retraining the model on the updated data.
    5. Documentation: The deployed machine learning model should be well documented to ensure that it can be easily understood and maintained over time. This may involve documenting the model architecture, input and output formats, and any specific requirements for the data pipeline or infrastructure.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/227794236-18214480-2ae5-41a1-8f44-27f3c68cb184.png" width="600" height="215" />
</p>

This is not an exhaustive list of steps to describe the workflow of an AI-based system but presents a high-level general view of the course of action along the way.
