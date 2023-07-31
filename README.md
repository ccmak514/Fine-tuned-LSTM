# Different Kernel Initializers and Optimizers on a Fine-tuned LSTM Model

<font size=3>In this AASD4011 project, IMDB dataset of 50K movie reviews from Kaggle is analyzed in this notebook. Instead of using pre-existing solutions, we plan to construct our own model from scratch. <br>
<br>
In this notebook, we aim to assess the impact of <font color=red><b>kernel initializers</b></font> and <font color=red><b>optimizers</b></font> on the performance of a neural network model. To conduct this experiment, all the hyperparameters, such as the number of neurons, layers, activation functions, and others, will remain constant. The variables we will manipulate are the <font color=red><b>kernel initializers</b></font> and <font color=red><b>optimizers</b></font>. The metric to evaluate the performance of the model is <font color=red><b>“accuracy”</b></font>.

In the initial stage of this project, we aim to perform data exploration to identify any missing or exceptional values in the dataset. Afterward, we will transform the categorical labels into numerical representations.<br>
<br>
Subsequently, our objective is to construct a baseline model, and fine-tune it to improve accuracy through changes in the number of layers, neurons, and other parameters except for the <font color=red><b>kernel initializers</b></font> and <font color=red><b>optimizers</b></font>. The <font color=red><b>default kernel initializer (glorot_uniform)</b></font> and <font color=red><b>adam optimizer</b></font> will be used in the baseline model.<br>
<br>
Finally, we will conduct an experiment to assess the impact of <font color=red><b>different combinations of kernel initializers and optimizers</b></font> on the baseline model's accuracy by using them as the only varying factors while all other hyperparameters remain unchanged.<br> 
<br>
The combinations of the following 2 hyperparameters will be examined.<br></font>

<font size=3>Kernel Initializer: 
- Glorot Uniform Initialization
- Glorot Normal Initialization
- He Uniform Initialization
- He Normal Initialization
- LeCun Normal Initialization
- Self-defined Initialization (details will be discussed)</font>

<font size=3>Optimizer:
- Adam
- RMSProp
- SGD</font>

<font size=3>The main takeaways from this notebook:
- Explore, preprocess and encode the dataset 
- Build a baseline model
- Examine combinations of above kernel initializers and optimizers (totally 18 combinations) by the baseline model
- Evaluate the train accuracy, validation accuracy, test accuracy of all combinations
- Evaluate the train loss, validation loss, test loss of all combinations</font>

### <b>Data - IMDB Dataset of 50K Movie Reviews</b>
<font size=3>The link of Kaggle:</font>
https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews
