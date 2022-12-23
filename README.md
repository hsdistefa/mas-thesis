# Predicting Long-Term U.S. Housing Price Trends Using a Long Short-Term Memory Neural Network

UCLA Master's Thesis, Copyright 2022

Full Paper [here](https://github.com/hsdistefa/mas-thesis/blob/master/manuscript/Harrison_DiStefano_MAS_Thesis.pdf)



## Abstract
Housing prices affect everyone. In this paper we establish a potential method of predicting long term home sale prices in the United States using an LSTM neural network model. We took publicly available macro economic data, then massaged it into a manageable form using cubic spline interpolation and logarithmic differencing. We then introduce the LSTM model using feature standardization, min-max normalization, and an Adam optimizer for backpropogation. After training the network on preceding data, we found that the network was able to provide predictions that coincided with similar market movements.

## Model Architecture

We use a multivariate LSTM neural network to model housing prices across time using various macro economic factors to predict future trends. Below is a flow diagram of the recurrent and unfolded architecture of the LSTM with inputs $x^{(t)}$ and predictions $\hat{y}^{(t)}$ at time $t$ with weights $U$, $V$, and $W$.

![LSTM Architecture](figures/lstm_architecture4.png)

Where the circles with diagonal lines represent standard LSTM memory cells with input, output, and forget gates.





