# Lumped-Deep-Learning
The topic proposes a new machine learning algorithm, called the lumped deep learning algorithm, using the pseudo-inverse and its residue to backpropagate and train the neuron weights.


The algorithm relies on the matrix operators, which can be easily implemented with the existing libraries such as EIGEN or LINPACK with high computational efficiency. Needed no gradient information, the loss function and the error function can be defined in many ways without causing much burden on the computational complexity. Since the pseudo inverse is intrinsically a least square method, the loss function may be chosen as the maximum standard deviation error among the training examples. Comparing the average error with the maximum error, we can justify whether the size of a neural network is proper for a specific machining learning task. The pseudo-inverse and its residue is backpropagated with low learning rates to make the annealing process of neural weights causing all examples to gradually agreed. When the number of layers and neurons can be determined by the number of independent training examples, the neural network can be easily configured without much trial effort. The city development prediction is used as an example, which involves the prediction of the population growth and the regional GDP growth. Despite the data discrepancy for the pseudo-inverse method, the lumped deep learning can still integrate different categories of data and consolidate them to perform the prediction. The result is compared with the conventional regression analysis, a significant improvement was found and discussed in the paper.


# Algorithm Flowchart
![Flowchart](https://github.com/blackbriar07/Lumped-Deep-Learning/assets/64767006/25f09e15-1dbc-447f-b397-07584895e166)

To perform an example, refer to the Lumped Deep Learning (pdf.) file uploaded. Follow step by step to get the results.


# Comparison with Google Tensorfloe Keras
The Lumped DNN verifies that given the layers and neurons can only attain 7 training data. If the number of data increases, the error standard deviation shoots up drastically. The resullt is verified using Google Tensorflow Keras.
![Comaprison](https://github.com/blackbriar07/Lumped-Deep-Learning/assets/64767006/38ed5665-f376-433e-99b5-7155a86d08e0)

# Conclusion
we propose a novel lumped deep learning algorithm using the pseudo-inverse methods in the backward propagation to locate the least square fitting for training neurons in the network, which differs from other conventional ML techniques adopting the gradient descent algorithm in the backward propagation. Considering the pseudo-inverse is intrinsically a least square fitting to the entire training set, we used the entire training set as a whole lump throughout the process.  As such, we named this novel method as the lumped learning. 
The lumped neural network needs minimally two hidden layers in the neural network. In the undisclosed experiments, we had tested many three hidden layers networks and found no significant improvement to the output errors. We apply this lumped deep learning technique to forecast the trend of city development in Guangdong, China as illustrated in Section 2 and 3.  Our results are approximate to what had happened in the real world.  In section 5, the comparison of our prediction results to that of the well-known google Tensorflow using the standard test case show that our method is computationally competitive in terms of the flow control based on the column permutation property.
Overall, this lumped deep learning algorithm with its distinctive annealing process can more quickly generate an optimal yet global solution among a massive amount of time series data as its calculation locates the least square error between the inputs and the outputs of the entire training set, largely reducing computational costs.
     However, we are still subject to some limitations.  According to the maximum neuron property of the lumped DNN learning, the regional GDP data for incorporating all 20 cities is deficient. Adding the population data into the training set, we found that the neural network performed well for 17 cities. The reason for the sound result may be due to their positive correlation. There are still more than 100 items could be used including the number of enterprises, the food production, number of teachers in the school and the like. Future research shall include the computational efficiency, the convergence and the neural network structure when we integrated more data together. The technique imitates the mini-batch used in the gradient method may be explored in the future.  
