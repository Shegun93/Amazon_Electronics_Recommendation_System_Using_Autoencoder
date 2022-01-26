# Recommendation Syetem Overview
A recommender system is simply an information filtering system. By drawing from huge data sets, the system’s algorithm can pinpoint accurate user preferences. Once you know what your users like, you can recommend them new, relevant content. And that’s true for everything from movies and music, to romantic partners

# Autoencoders
Autoencoders are a specific type of feed forward neural networks where the input is the same as the output. They compress the input into a lower-dimensional code and then reconstructs the output from this representation. The code is a compact “summary” or “compression” of the input, also called the latent-space representation. Auto encoders are great feature extractors because of their highly compressing representation of data (Zhang et. al, 2019). 
An autoencoder consists of 3 components: encoder, codes and decoder. The encoder compresses the input and produces the code, the decoder then reconstructs the input only using this code. Its data compression ability make it an important method in feature extraction; recommendation systems relied heavily on data reconstruction and that explains our choice of deep neural network and autoencoder in particular.

# Autoencoder For Recommendation System
Recommendation system with autoencoder have proven in performance to be the best compare to other state of the art model; most approaches for recommendation system are based on training algorithms such as KNN. Deep Learning is the strengthening area for recommendation systems research (Vito et al). Several deep learning techniques are applied in collaborative filtering are Convolutional neural networks, recurrent neural networks and deep neural networks and suggested to use distributed optimization techniques for minimizing computational cost (Jindal. et al). More concentration done on the performance of the recommendation systems but (F.Yuan.et al) explain the issues of data contamination solved by Autoencoder. The experiment shows a very low RMSE value and considering that the recommendations presented to the users are in line with their interests and are not affected by data sparsity problem.

# Data Description
Amazon Reviews data (data source) The repository has several datasets. For this case study, we are using the Electronics dataset.

# Domain
E-commerce

# Context
Online E-commerce websites like Amazon, Flipkart uses different recommendation models to provide different suggestions to different users. Amazon currently uses item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real-time.
Looking to train amazon electronics dataset with autoencoder following collaborative filtering method. The Collaborative Filtering Recommender is entirely based on the past behavior and not on the context. More specifically, it is based on the similarity in preferences, tastes and choices of two users. It analyses how similar the tastes of one user is to another and makes recommendations on the basis of that.

# Data Attributes
Attribute Information:

1.  userId : Every user identified with a unique id
2.  productId : Every product identified with a unique id
3.  Rating : Rating of the corresponding product by the corresponding user
4.  timestamp : Time of the rating (Maybe Ignore)

# Requirements
1.  Pytorch
conda install -c pytorch pytorch
2.  Pandas
pip install pandas
3.  Numpy
pip install numpy



