# Rainfall-fore-casting
Models used: Gated Reccurent Unit,Long Short Term Memory,Reccurent Neural Network  We proposed an optimized GRU neural network model for regional rainfall forecasting using a data set.  Constructed and compared different models to analyze and compare (GRU,LSTM,RNN)
1.	Optimal Planting Schedule: Farmers need to know when to plant their crops for the best possible yield. and to select the type of crop,according to predicted rainfall
2.	Rainfall forecasting enables farmers to plant their crops just before rains are expected.
3.	Rainfall forecasts help farmers decide when to harvest, taking into account the risk of rain damage during the harvest period
4.	We proposed an optimized GRU neural network model for regional rainfall forecasting using a dataset from climate knowledge portal. ---from 1991 to 2020
Dataset parameters: Temperature, Rainfall, ghg, ch4

5.	we also constructed and compared different  models(RNN,LSTM,GRU) to analyze, compare, and evaluate the advantages of selected methods in terms of real-time forecasting over the same dataset.
6.	In a simple RNN, each input data point is processed sequentially, and the network maintains an internal state that carries information from the previous steps to the current one.
7.	Backpropagation (short for "backward propagation of errors") is a fundamental algorithm used in training artificial neural networks. It's a supervised learning technique that helps adjust the model's parameters, such as weights and biases, to minimize the difference between the predicted output and the actual target output
8.	However, simple RNNs can suffer from vanishing gradient problems,
9.	The vanishing gradient problem is a challenge that emerges during backpropagation when the derivatives or slopes of the activation functions become progressively smaller as we move backward through the layers of a neural network.
10.	GRU neural network
a.	GRU performs similar to the LSTM model
b.	GRU comprises the update and reset gate to overcome the problem of vanishing gradients of a typical RNN model
c.	The update gate controls how much of the past memory to preserve
d.	reset gate specifies how to merge the previous memory with the fresh input.
11.	Long Short-Term Memory (LSTM) Networks
a)	LSTMs have a more complex structure that allows them to capture and retain information for longer periods.
b)	Here we have three gates: forget gate,input gate,output gate
c)	Forget Gate: This gate determines what information from the previous state should be discarded or forgotten. It takes the previous state and the current input and produces a value between 0 and 1 for each element in the memory cell. A value of 0 means "completely forget," while a value of 1 means "keep everything."
d)	Input Gate: This gate decides what new information should be stored in the memory cell. It processes the current input and the previous state to create a new candidate value for addition to the cell.
e)	Output Gate: This gate controls what information should be read from the memory cell to produce the output.

12.	GRUs could provide a good balance between performance and efficiency.
13.	LSTM works good for large datasets and GRU can works with smaller datasets and can give accurate prediction
14.	study  found that GRU is 29.29 % faster and 23.45 % more precise compared to the LSTM neural network
Code part
15.	After uploading the dataset, next step is data preprocessing.
16.	Missing values in the dataset are dealt by replacing it with mean values. This helps to ensure that there are no gaps or inconsistencies in the data that could affect the accuracy of the rainfall forecasting.
17.	Normalization is applied to the data to bring all the input variables to a similar scale. This step is important because different atmospheric parameters may have different ranges and units. Normalization helps to prevent any single parameter from dominating the forecasting process. Common normalization techniques include Min-Max scaling and z-score normalization.
18.	Feature selection is performed to identify the most relevant and significant input variables for rainfall forecasting. This step helps to reduce the dimensionality of the dataset and eliminate any noisy or irrelevant features.
19.	Next, the pre-processed data is split into training, validation, and test sets to evaluate the accuracy of the proposed framework
20.	Correlation analysis is done to determine the relationship between variables and their impact on the rainfall variable.
21.	The proposed model achieved high prediction accuracy by maintaining minimal Normalized Mean Absolute Error (NMAE) and Normalized Root Mean Squared Error (NRMSE).


What is deep neural network or deep learning?
Deep learning is the branch of machine learning which is based on artificial neural network architecture. An artificial neural network or ANN uses layers of interconnected nodes called neurons that work together to process and learn from the input data.
In a fully connected Deep neural network, there is an input layer and one or more hidden layers connected one after the other. Each neuron receives input from the previous layer neurons or the input layer. The output of one neuron becomes the input to other neurons in the next layer of the network, and this process continues until the final layer produces the output of the networkWhat are the plants that  require less water and more water?
What is vanishing gradient problem?
22.	The vanishing gradient problem is a challenge that emerges during backpropagation when the derivatives or slopes of the activation functions become progressively smaller as we move backward through the layers of a neural network.
Where did u get the dataset from and what are the parameters of dataset?
We got data from climate knowledge portal and parameters are: temperature ,rainfall,ghg,ch4
Why you used only these parameters?
Why gru over LSTM..difference?
12.	GRUs could provide a good balance between performance and efficiency.
13.	LSTM works good for large datasets and GRU can works with smaller datasets and can give accurate prediction
14.	study  found that GRU is 29.29 % faster and 23.45 % more precise compared to the LSTM neural network
Drawback of RNN?
Ans. Vanishing gradient problem in RNN
What did you do to replace missing values in dataset and what are techniques used for replacing missing values?
Replaced it using mean values of the specified column
 
Data normalization technique? what are techniques used for data normalization
