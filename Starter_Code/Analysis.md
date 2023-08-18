Overview:
The goal of this project was to create a model that can accuratly predict whether a venture would be successful for Alphabet Soup. In order to get an in depth prediction, using a neural network model seemed to be a good choice.


Report:
Our model's target is the outcome of the venture. To determine this, we use the following features: Application type, affiliation, classification, use case, organization, status, income amount, special consideration and ask amount. The variables name and EIN were removed from our data for our initial analysis.

To start, we used rectified linear units as our activation function for our layers with the last one using sigmoid instead, three dense layers consisting of 49, 80, 30 and 1 neuron(s) each. This was just to give a starting point before optimization. Using this model, we achieved an accuracy of 61.82%. Next we moved to optimization. After testing many different combinations of activation functions, layers and neurons, the best outcome came with the following. First, we added the name variable back in. Then we stuck with rectified linear unit as our activation function for layers one and two with sigmoid as our output layer as well. For our neurons, we used 90 and 30 in our hidden layers respectively. This yielded an accuracy score of 78.36%, much better than our inital model.

Summary:
After optimizing our model, we were able to get an accuracy score of 78.36%. While this is by no means perfect, it's significantly better than what we stated with and over the accuracy goal of 75%. The drawbacks to this model are the compute times. Because we added names back into our feature variables, there are nearly two million parameters. Whether or not you use the model comes down to prioritizing time or accuracy.