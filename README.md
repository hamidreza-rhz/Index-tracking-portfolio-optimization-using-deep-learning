# Index-tracking portfolio optimization using Deep learning

Implementing a deep learning model with PyTorch framework to minimize the index-tracking portfolio loss to optimize the portfolio for better imitation of the S&P 500 index. We introduce a deep neural network, use a shallow neural network as the deep learning baseline, and the simple 1/N model as the benchmark. Then compare Deep NNF to other two models in form of full replication or partial replication of the index to find out the performance of our model.

## Paper Reference

This project is based on the paper:

Yuyeong Kwak, Junho Song, Hongchul Lee, "Neural network with fixed noise for index-tracking portfolio optimization," Expert Systems with Applications, Volume 183, 2021, 115298, ISSN 0957-4174

[Link to the paper](https://www.sciencedirect.com/science/article/abs/pii/S0957417421007284)

## Folder Structure
The project repository is organized as follows:

- data: This folder contains the necessary data files required to run the project.
- full_replication.ipynb: A Jupyter Notebook implementing full replication, which considers all possible stocks for tracking the S&P 500 index.
- partial_replication.ipynb: A Jupyter Notebook implementing partial replication, which considers a subset of stocks for tracking the S&P 500 index.
- getdata.ipynb: A Jupyter Notebook used for extracting necessary data
- tickerlist.csv: A CSV file containing the list of stocks used in the project.
- data.csv: A CSV file containing the close prices of the stocks.
- sp500.csv: A CSV file containing the close prices of the S&P 500 index.

##  Models

### Deep Neural Network (Deep NNF)
A neural network consisting of six fully connected layers and a ReLU activation layer between the fully connected layers. Applying dropout to each fully connected layer to prevent overfitting.

### Shallow Neural Network (Shallow NNF)
A neural network consisting of three layers: fully connected layer, ReLU activation layer, and fully connected layer

### 1/N Model
Equally weighted portfolio which gives the 1/N weight (N being the number of stocks) to each stock and does not distinguish between the stock's importance

## Additional Info
Please refer to the respective Jupyter Notebook files for a detailed implementation and analysis of the index tracking portfolio optimization using deep learning.

Feel free to explore the project and use the provided code as a starting point for your own research or portfolio optimization experiments.
