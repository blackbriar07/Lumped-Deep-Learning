# Lumped-Deep-Learning
The topic proposes a new machine learning algorithm, called the lumped deep learning algorithm, using the pseudo-inverse and its residue to backpropagate and train the neuron weights.


The algorithm proposes a new machine learning method called lumped deep learning, which utilizes the right pseudoinverse projection for weight learning and the left pseudoinverse projection to generate residue for training the preceding hidden layers in a backpropagation process. The method relies on matrix operators that can be easily implemented using existing libraries such as EIGEN or LINPACK, ensuring high computational efficiency. The pseudoinverse is inherently a least squares method, requiring no gradient information. Lumped deep learning backpropagates its projected error residues with a chosen learning rate to facilitate the annealing process in training neural weights, essentially performing layer-to-layer projection. This layer-to-layer projection forms a hierarchical committee machine that can be used in symbiosis analysis, akin to game theory analysis, within the state-transition model at specific instances in time. The lumped deep learning method first determines the number of layers and neurons based on the number of independent training examples without the need for additional network optimization efforts. This method can integrate heterogeneous data such as GDP and population to perform symbiosis analysis. The city development symbiosis analysis involves analyzing the synergy between population growth and regional GDP growth in different cities. This analysis is obtained by deriving a state-transition dynamic model using lumped deep learning. In this paper, we study the symbiosis analysis of city development in Guangdong province.


# Algorithm Flowchart
![Flowchart](https://github.com/blackbriar07/Lumped-Deep-Learning/assets/64767006/25f09e15-1dbc-447f-b397-07584895e166)

To perform an example, refer to the Lumped Deep Learning (pdf.) file uploaded. Follow step by step to get the results.


# Comparison with Google Tensorflow Keras
The Lumped DNN verifies that given the layers and neurons can only attain 7 training data. If the number of data increases, the error standard deviation shoots up drastically. The resullt is verified using Google Tensorflow Keras.
![Comaprison](https://github.com/blackbriar07/Lumped-Deep-Learning/assets/64767006/38ed5665-f376-433e-99b5-7155a86d08e0)

# Conclusion
We propose a lumped deep learning algorithm using pseudo-inverse methods in backward propagation to achieve least square fitting for training neurons in the network. This approach differs from the PIL algorithm, which only adopts the feedforward process, and from other conventional machine learning techniques that require the gradient descent algorithm. By precisely defining the use of the right pseudo-inverse and left pseudo-inverse in different contexts, we enable the replacement of the computationally less efficient SVD method with the highly efficient, reliable, and readily available LUP matrix decomposition algorithm. 

The lumped neural network requires a minimum of two hidden layers. In undisclosed experiments, we tested several networks with three hidden layers and found no significant improvement in output errors. Comparing our prediction results to those of the well-known Google Tensorflow using standard test cases shows that our method is computationally competitive, particularly due to its flow control based on the column permutation property. Overall, this lumped deep learning algorithm, with its distinctive annealing process, can quickly generate an optimal yet global solution among massive amounts of time series data. Its calculation locates the least square error between the inputs and the outputs of the entire training set, significantly reducing computational costs.

Thanks to the pseudo-inverse projection nature, we are able to analyze the synergy forces among cities in the study of city development. According to the symbiosis analysis, we concluded that cities such as Guangzhou, with diversified economic activities, are more self-sustainable than export-oriented cities. Meizhou, with its industry long dominated by a low-process, natural resource-dependent "heavy-weighted" structure, needs a transformation to adapt to first-tier cities as well as its neighboring cities.

Future research should focus on improving computational efficiency, investigating convergence, and optimizing neural network structures when integrating additional economic data.


