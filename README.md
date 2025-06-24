# K-Nearest Neighbors (KNN)
K-Nearest Neighbors (KNN) is a supervised machine learning algorithm used for classification and regression tasks. It is one of the simplest yet powerful algorithms in machine learning.
KNN works on the principle that similar data points exist close to each other in a multidimensional space. It classifies a new data point based on the majority class of its 'K' nearest neighbors.
**📚 Key Concepts**
**1. Instance-Based Learning**
KNN is called a lazy learner: It doesn’t learn an explicit model during training.

Instead, it stores the entire training dataset and performs classification only when it sees new data (on-the-fly computation).

**2. Distance Metric**
To find the 'nearest' neighbors, KNN uses a distance function, such as:

**Euclidean Distance (most common):**
𝑑(𝑝,𝑞)=  ∑𝑖=1𝑛(𝑝𝑖−𝑞𝑖)2
d(p,q)= i=1∑n(pi−qi) 2
 
​
 
**Manhattan Distance:**
𝑑(𝑝,𝑞)=∑𝑖=1𝑛∣𝑝𝑖−𝑞𝑖∣
d(p,q)=i=1∑n∣pi−qi∣


**🛠️ How KNN Works**
Step-by-Step:
Choose the value of K (e.g., 3, 5, 7)

Calculate the distance from the test point to all training data points.

Select K closest data points (the neighbors).

Classify (or predict) based on:

Classification: Majority voting among the K neighbors.

Regression: Averaging the output values of the K neighbors.

📊 Example (Classification)
Suppose you're classifying fruit as apple 🍎 or orange 🍊 based on weight and texture.

New fruit: Weight = 150g, Texture = smooth

K = 3

Find 3 closest fruits in the dataset

Suppose: 2 apples, 1 orange → predict: apple

**✅ Advantages**
Simple to understand and implement

No training phase (good for real-time systems with small data)

Works well with well-separated classes

**❌ Disadvantages**
Slow with large datasets (requires computation for all training points)

Sensitive to irrelevant features and feature scaling

Curse of dimensionality: Becomes less effective as the number of features increases

Performance depends heavily on the choice of K and distance metric



