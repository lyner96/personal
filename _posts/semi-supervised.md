Semi-supervised learning aims to combine supervised and unsupervised learning. Typically, it attempts to improve performance in one of these two tasks by utilizing information generally associated with the other. Semi-supervised classification methods are particularly relevant to scenarios where labelled data is scarce. If sufficient unlabelled data is available and under certain assumptions about the distribution of the data, the unlabelled data can help in the construction of a better classifier. [1]

When you don’t have enough labeled data to produce an accurate model and you don’t have the ability or resources to get more data, you can use semi-supervised techniques to increase the size of your training data. You can use a semi-supervised learning algorithm to label the data, and retrain the model with the newly labeled dataset. However, there is no way to verify that the algorithm has produced labels that are 100% accurate, resulting in less trustworthy outcomes than traditional supervised techniques. [2]



The basic procedure involved is that first, the programmer will cluster similar data using an unsupervised learning algorithm and then use the existing labeled data to label the rest of the unlabelled data. Semi-supervised assume the following: [3]
1. Continuity Assumption: The algorithm assumes that the points which are closer to each other are more likely to have the same output label.
2. Cluster Assumption: The data can be divided into discrete clusters and points in the same cluster are more likely to share an output label.
3. Manifold Assumption: The data lie approximately on a manifold of much lower dimension than the input space. This assumption allows the use of distances and densities which are defined on a manifold.

Taken from:
1. Van Engelen, J. E., & Hoos, H. H. (2020). A survey on semi-supervised learning. Machine Learning, 109(2), 373-440.
2. [DataRobot ~ Semi-Supervised Machine Learning](https://www.datarobot.com/wiki/semi-supervised-machine-learning/)
3. [GeeksforGeeks ~ Semi-Supervised Learning](https://www.geeksforgeeks.org/ml-semi-supervised-learning/)