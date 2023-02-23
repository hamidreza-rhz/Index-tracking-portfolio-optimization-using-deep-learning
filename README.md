# Index-tracking portfolio optimization using Deep learning

Implementing a deep learning model to minimize the index-tracking portfolio loss to optimize the portfolio for better imitation of the S&P 500 index. We introduce a deep neural network, use a shallow neural network as the deep learning baseline, and the simple 1/N model as the benchmark.

This project is based on the paper:
Yuyeong Kwak, Junho Song, Hongchul Lee,
Neural network with fixed noise for index-tracking portfolio optimization,
Expert Systems with Applications,
Volume 183,
2021,
115298,
ISSN 0957-4174

https://doi.org/10.1016/j.eswa.2021.115298
https://www.sciencedirect.com/science/article/pii/S0957417421007284

##  Models

### Deep Neural Network (Deep NNF)
A neural network consisting of six fully connected layers and a ReLU activation layer between the fully to each fully connected layer to prevent overfitting.

### Shallow Neural Network (Shallow NNF):
A neural network consisting of three layers: fully connected layer, ReLU activation layer, and fully connected layer

### 1/N Model
Equally weighted portfolio which gives the 1/N weight (N being the number of stocks) to each stock and does not distinguish between the stock's importance