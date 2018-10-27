# KNearestNeighbours
Implementing KNN to classify handwritten digits from MNIST from scratch

KNN is probably one of the most simple and intuitive classification algorithm.

Consider a training set {Xi,Yi}, where Xi is the feature vector of the ith training sample, and Yi is the class label of the same.
Xi is a 1xN vector, where N is the number of features of the sample. In case of MNIST classification problem, each pixel is a feature of a training example.

These features are, in mathematical terms, simply points on an N-dimensional hyper plane.

In KNN, consider a test example. This can also be represented as a point in the N-dimensional hyper-plane.

We find the K closest points in the hyper plane (K can be any integer above 1) using a distance metric (such as L0,L1,L2,Chebyshev distance). In this example,L2 or Euleclidian distance is used.

The cass labels Yi, for these K closest points (hence the name K-Nearest Neighbours) in the hyper-plane are found, and the test example is classified as that class which has the highest frequency among the K examples.

An exampleof a classification problem in 2D space is as shown below:
![knn-1](https://user-images.githubusercontent.com/42526509/47608158-624d4b80-d9de-11e8-8b69-49bbb45d8e87.png)

When K=3, the class label assigned to test example (denoted by ?) is that of the dotted triangle,because of the three closest neighbours, the dotted triangles are the majority.

When K=11, the class labelis that of filled triangle. In this case, the filled triangles are the majority amongthe 11 closest neighbours to the test example.
