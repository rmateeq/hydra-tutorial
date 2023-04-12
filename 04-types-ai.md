## Types of AI

AI is a broad term that has evolved. The purpose here is to understand the necessary types of artifacts, constructs, and models that AI provides to make software applications intelligent. Although, this list is long, let's confine the discussion to two broad categories, namely rule-based AI and machine learning.

### Rule-based AI
Rule-based AI is considered a simple technique that tries to represent the domain knowledge and inference rules to conclude. For example, consider the situation where we need to represent the rule "all men are mortal" in a way that we can be used to draw new inferences. It can be represented using the following predicate logic:

- ∀ X man(X) → mortal(X) (read as "for all X, if X is a man, then X is mortal". Here X is a variable)

This rule can be used in combination with domain knowledge to draw inferences. For example:

- man(Socrates) (read as "Socrates is a man")

This predicate can be used with the above rule to draw the inference that "Socrates is mortal".

The major limitation of this rule-based AI is that it can be used to build deterministic systems only where the data is small and the rules are clear. Such systems cannot learn new things themselves.

### Machine Learning
Machine learning on the other hand can define its own rules based on data. The system can learn and adapt as new data emerges. This capacity to learn and adapt has made machine learning the most popular choice while integrating intelligence into software systems.
As an example, let's consider the question [this example is taken from Sebastian Thun's Intro to ML course on Udacity]

- "is horse an acerous?"

What is an acerous? Well, instead of answering this question directly, let's have a few examples that can help us learn this.

- An elephant is acerous
- A ram is non-acerous
- A triceratops is non-acerous
- A lemur is acerous
- A dog is acerous
- A giraffe is non-acerous
- A goat is non-acerous
- A cat is acerous
- A parrot is acerous
- A deer is non-acerous

Before answering this question, let's discuss the approach. We need to look at different features to decide. These features could be color, number of legs, horns, etc. And it happens that a horse is an **acerous**. Why? Because a horse does not have either horns or antlers. Whereas, all the animals in the non-acerous group have. This demonstrates the process and capability of machine learning to learn something new by itself as new data emerges. 

Machine learning is further classified into different categories. Although, it is a vast developing debate, however, some popular approaches are listed below:

1. Supervised Learning
2. Unsupervised Learning
3. Recommender Systems
4. Anomaly Detection
5. Reinforcement Learning

Let's discuss these types in slight detail.

#### Supervised Learning
It is widely believed that most of the value that machine learning is generating is coming from supervised learning. In this approach, the historical data is available with true answers. A model is trained on that data to learn the general pattern in the data and is later used to predict the cases where the true answer is not known. The example of "horse being acerous" perfectly fits in this category because we knew different animals whether they were acerous or not. Through those examples, machine learning would somehow generalize the facts that lead to the conclusion of another (initially uncategorized) animal being acerous or not. 

Supervised learning is further divided into two sub-categories: classification, and regression. In classification, the output is categorical and limited. In the example of a horse being acerous or non-acerous, the output is categorical and we are trying to classify an animal into a pre-defined set of classes (which in this case are two). In regression, the output is continuous. A common example is to predict house prices based on different features like area, number of bedrooms, etc.

#### Unsupervised Learning
Like supervised learning, unsupervised learning also bases its outcomes on data. However, unlike supervised learning, the data is not labeled or the true answers are not known. One of the most common examples of unsupervised learning is news article grouping or clustering based on common terms and/or themes. As a more tangible case, Google groups news articles from various sources and publishers based on common terms. Anomaly detection often also falls under unsupervised learning.

#### Recommender Systems
Recommender systems can be based on either or both supervised or unsupervised learning. Considering the growing usage, and demand, many experts treat recommender systems as a special category in machine learning. In a supervised learning approach, the model is trained on labeled data where the target variable is the item that the user has previously interacted with (e.g. watched, bought, etc.). The model then predicts what items the user might be interested in based on the previous interactions. Whereas, in unsupervised learning, the model tries to identify patterns in the user's behavior without being explicitly told what the user might be interested in. The model then recommends items based on the identified patterns.

#### Reinforcement Learning
Unlike supervised and unsupervised learning, in reinforcement learning, there is no historical data to learn from. An agent learns to make decisions by interacting with the system in real time. The system uses rewards for good decisions and penalties for bad decisions. Playing chess or any other game as well as self-driving cars use reinforcement learning to improve performance over time. In chess, an agent (player) can make moves and receive a reward for making good moves and a penalty for making bad moves. Over time, the agent will learn to make better moves based on the rewards and penalties it receives, eventually leading to it becoming a skilled chess player.

In the following table, we list a few primitive examples of supervised, unsupervised, and reinforcement learning.


<p align="center">
  
|Learning Type|Sub-Category|Example|
|----------|----------|----------|
|Supervised|Classification|Predicting if an email is a spam or not based on its content.|
|Supervised|Classification|Predicting a disease based on a patient's record.|
|Supervised|Regression|Predicting the price of a house based on its features such as number of rooms, location, and square footage, etc.|
|Supervised|Regression|Predicting stock price based on company's data and market trends, etc.|
|Unsupervised|Clustering|Grouping customers into different segments based on their purchasing behavior.|
|Unsupervised|Anomaly Detection|Detecting fraudulent transactions in a financial dataset.|
|Unsupervised|Recommender System|Recommending movies by the grouping of users based on similar interests.|
|Reinforcement||An agent can learn to pick up a box and place it on a table by receiving a positive reward for completing the task and a negative reward for dropping the box.|

</p>

### Deep Learning
Having discussed primary categories of machine learning with some brief examples, it is inevitable to mention deep learning to complete the discussion. Deep learning has taken to the world by storm recently by leveraging its capability to learn in systems involving massive and complex data. Deep learning is being used to realize some amazing applications in computer vision, speech recognition, natural language processing, and generative models (that can generate new data based on existing data).

Deep learning harnesses the power of deep neural networks to effectively solve complex problems that other types of machine learning falls short of. In the following, some popular types of deep neural networks are listed.

#### Feedforward Neural Networks (FFNNs)
FFNN are a type of artificial neural network where the information flows in a single direction, from the input layer to the output layer. The FFNN banks of backpropagation to complete the training. It is sometimes called multi-layer perceptrons because they consist of multiple layers of perceptrons. FFNNs are commonly used for pattern recognition, regression, time series analysis, natural language processing, and recommendation systems.

#### Convolutional Neural Networks (CNNs)
CNNs are a type of neural network that are particularly effective for processing and analyzing data with a grid-like structure, such as images or audio signals. Unlike feedforward neural networks, which process input data in a single pass through a series of layers, in CNNs the convolutional layers apply a set of filters to the input data, which extract different features at different spatial locations in the input. Common applications of CNNs include image classification, object detection, face recognition, speech recognition, and medical image analysis.

#### Recurrent Neural Networks (RNNs)
RNNs (including long short-term memory: LSTM) are a type of neural network that are particularly effective for processing sequential data, such as time series or natural language text. In contrast to convolutional neural networks, which are particularly effective for processing grid-like data such as images, RNNs are particularly effective for processing sequential data. While CNNs use convolutional layers to extract features from the input data, RNNs use loops in their architecture to capture temporal dependencies in the input data. In contrast to feedforward neural networks, which process input data in a single pass, RNNs use feedback loops to allow information to persist over time. Some particular applications of RNNs are language modeling (e.g., predict the probability distribution over the next word in a sequence of words), speech recognition, time series analysis (e.g., predicting stock prices or weather patterns), and machine translation.

#### Generative Adversarial Networks (GANs)
GNNs are a type of neural network architecture that consists of two networks: a generator and a discriminator. The generator learns to produce synthetic data that is similar to real data, while the discriminator learns to distinguish between real and fake data. GANs are typically used for generative modeling tasks, where the goal is to learn a probability distribution over the data and generate new samples from it. Some prominent applications of GANs are image, video, and text generation; drug discovery, and game design.

#### Tranformer based Models
Transformers are a type of neural network architecture that have gained popularity in recent years, particularly for natural language processing. Unlike CNNs and RNNs, which operate on fixed-length inputs, transformers can handle variable-length sequences of inputs. Transformers are designed to capture long-range dependencies in sequential data by using a self-attention mechanism. This allows the model to attend to different parts of the input sequence at different time steps, and has been highly successful in NLP tasks such as language translation, question-answering, and text generation. Some popular transformer-based models include GPT (Generative Pre-trained Transformer), BERT (Bidirectional Encoder Representations from Transformers), T5 (Text-to-Text Transfer Transformer), and ViT (Vision Transformer).

#### Diffusion Models
Diffusion models are a class of probabilistic generative models that have recently gained popularity in the deep learning community. Unlike traditional deep learning models that are designed to perform specific tasks such as classification or prediction, diffusion models are used to model complex probability distributions over high-dimensional data, such as images or video. One of the main advantages of diffusion models is their ability to generate high-quality samples from complex distributions, which makes them well-suited for applications such as image and video generation, data augmentation, and anomaly detection. Some recent applications of diffusion models are image generation, video generation, and data augmentation.

The following table summarizes the popular deep learning models and their applications.

<p align="center">

|Model Name|	Model Type|	Example|
|---------|---------|---------|
|Feedforward Network|	Supervised|	Image classification, text classification, regression|
|Convolutional Network|	Supervised|	Image classification, object detection, segmentation|
|Recurrent Neural Network|	Supervised|	Time-series analysis, text analysis, speech recognition|
|Generative Adversarial Network|	Unsupervised|	Image synthesis, data augmentation, anomaly detection|
|Transformer-based Model|	Supervised/Unsupervised|	Language translation, text generation, image captioning, question answering|
|Diffusion Model|	Unsupervised|	Image synthesis, video synthesis, anomaly detection, image inpainting|

</p>
  
In the next section, we turn our attention to some popular use cases of different types of AI.
