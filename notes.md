# Machine Learning - Understanding Tensor Flow

## Introducing TensorFlow

Machine Learning Problems:

- Classification 
- Regression (fitting curve to data)
- Clustering (Grouping data based on similarities)
- Rule-Extraction (if-then patterns)

Example:
Whales Classification: Are they mammal or fish
- Rule-based classfier
  - A series of rule created by experts
- ML-based Classifier
  - Creates classifier based on corpus of already tagged data
  - Information about input data is critical when trying to compare with known data
  - Very dependent on features of the training data and features of input data
 - Difference between the two types:
  - ML Based is Dynamic vs rule-base which is static
  - ML Based dont really require experts, rule-based require experts
  - ML Based reqiure a corpus of data
  - ML Based has a training step

Traditoinal ML based binary classifier
- input is a vector of features
- output is classification (label)
Modern "Representation" classifiers
- automatically determine input feature vectors

## Understanding Deep Learning

- Representation systems can figure out feature and classifications by itself during training
- The Key to the the "representation" system is the feature selection algorithm

## Deep Learning and Neural Networks

- Deep Learning: Algorithms that learn what features matter (widely used for speach and image recognition)
- Neural Networks: The most common class of deep learning algos
- NN are built up of Neurons, which are the building blocks to support "learning"

- Deep Learning systems are made up of layers:
  Example: Image Recognition
  - Pixel extraction
  - Edge Extraction
  - Corner Extraction
  - Object Part combination
 The input and output layers are the visible layers
 The middle layers are the hidden layers

 ## Introduction Of Tensorflow
 - Open source library for numerical computation using data flow graphs,
 made by Google
 - Build for distributed world (clusters, GPUS, etc)
 - Suite of software (TensorFlow Board, serving)

 ### Uses:
  - Greate for ML development
  - Has a REPL env for quick development
  - Models are easily ported to production
  - Large scale distributed models
  - Models for mobile and embedded envs

 ### Strengths

 - Easy to use Stable Python Api
 - Scalable
 - Efficient and performant
 - Great support from Google
 - Addional tools for viz and serving

### The World is a Graph

- Everything is a graph either a node or an edge
- Every node is a computation/operators
- Every edge is Data, data is transformed by nodes, also called tensors

Example: (Flow Grap)

----1.8----(round)--2--(multiply)--10--(add)--15
              \       /               /
               2     5               5
                \   /               /  
--3.6--(flr)--3-(add)----5-----(abs)


