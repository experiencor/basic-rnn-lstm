These are the barebone implementations of vanilla RNN in numpy and LSTM in tensorflow to highlight the process of backpropagation through time [1]. They are then demonstrated for both character-based and word-based text generation. The backpropagation through time (BPTT) of RNN follows the manually derived derivatives while LSTM relies the auto-differentiation capability of tensorflow. The BPTT of RNN can be truncated. However, the BPTT of LSTM cannot be truncated due to the limitation of tensorflow's auto-differentiation in looping control.

Example character-based texts generated by LSTM:

```
him, foremoble, as he wife thou art many than it is a cannot leaved; comef's riched, of their good ti

leave on me; you shall I think frown.
```

A lot more training is needed to produce better results.

Resources for conceptual explainations:
1. http://www.wildml.com/2015/09/recurrent-neural-networks-tutorial-part-1-introduction-to-rnns/
2. http://colah.github.io/posts/2015-08-Understanding-LSTMs/

# Usage

1. "Basic RNN.ipynb" => walk-through implementation of vanilla RNN in numpy, user-defined truncated BPTT
2. "Basic LSTM.ipynn" => walk-through implementation of LSTM in tensorflow, only full BPTT implemented due to limitation of tensorflow