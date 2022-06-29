# LSTM Neural Network

LSTM built using the Keras Python package to predict stock price.

---

## Requirements

Install below requirements to make sure correct versions of libraries are being used.

- numpy 1.22.0
- pandas 1.3.5
- scikit-learn 1.0.2
- tensorflow
- keras 0.7.0
- matplotlib 3.5.1
- matplotlib-inline 0.1.3

---

## Theoretical Background Knowledge (notes)

---

| Sr. No. | Concepts Covered        |
| ------- | ----------------------- |
| 1.      | Deep Learning           |
| 2.      | Recurent Neural Network |
| 3.      | Long short-term memory  |
| 4.      | Bidirectional LSTM      |

---

## 1. Deep Learning

"Deep Learning is a subfield of machine learning concerned with algorithms inspired by the structure and function of the brain called artificial neural networks." There are different types of DL models: Convolutional Neural Network, Recurrent Neural Networks (RNN), Long Short Term Memory (LSTM), Restricted Boltzmann Machine (RBM), Deep Belief Networks, etc.

---

## 2. Recurent Neural Network

Recurent Neural Network is a type of DL model that is mostly used for analysis of sequential data (time series data prediction).

---

## 3. LSTM

In order to address the long-term information preservation and shor-term skipping in latent variable model, we use LSTM. It allows a neural network to remember the stuff it needs and forget that is no longer applicable.

It is a special type of RNN, capable of learning long-term dependencies. LSTM provides the solution to the long term dependency problem of RNN by adding 'internal state' to the RNN node.

The internal state contains following 3 parts
|1|2|3|
|--|--|--|
|Forget Gate|Input Gate|Output Gate|
|Says what information stored in the internal state can be forgotten i.e. no longer contextually relevent|what new information should be added or updated into the working storage state information|Says out of all the stored information what information should be outputed in the perticular instance
|

## 4. Bidirectional LSTM

Bidirectional LSTM model improves performance on a sequence classicication problem. It encodes the sequence in the forward as well as backword direction, and concatinates the result from both the forward LSTM and backward LSTM for each timestamp.

---

## Resources: <a name="Resources"></a>

- [LSTM Original Paper](https://www.bioinf.jku.at/publications/older/2604.pdf)
- Keras: [https://keras.io/](https://keras.io/)
- Tensorflow: [https://www.tensorflow.org/](https://www.tensorflow.org/)
- [LSTM in Detail](http://colah.github.io/posts/2015-08-Understanding-LSTMs/)
