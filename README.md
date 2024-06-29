                                                    Word Embedding Training with Context Pairs


This project demonstrates a simple implementation of word embeddings using a small vocabulary and context pairs. The code trains word vectors using a basic neural network approach similar to the Continuous Bag of Words (CBOW) model.

Description:
The project is designed to learn word embeddings for a small vocabulary based on context pairs. It uses a simple neural network to map words to vectors in a continuous vector space. The training process involves forward and backward passes to adjust the weights, ultimately minimizing the prediction error for context words given a center word.

Key Components:
Vocabulary and Context Pairs: Defined a small vocabulary and context pairs to train the embeddings.

One-Hot Encoding: Used one-hot encoding to represent words as vectors.

Weight Initialization: Initialized weights for the input-to-hidden and hidden-to-output layers.

Softmax Function: Applied softmax to the output layer to obtain probability distributions.

Training Loop: Iterated over the context pairs to update the weights and minimize the loss using cross-entropy.

Training Process:
Data Preparation: Gathered a small set of context pairs from the vocabulary.

One-Hot Encoding: Converted words into one-hot vectors for processing.

Forward Pass: Calculated the hidden layer and output probabilities for each center word.

Loss Calculation: Used cross-entropy to measure the prediction error.

Backward Pass: Computed gradients and updated the weights to minimize the error.

Iterations: Repeated the process for a set number of epochs to ensure convergence.

Evaluation:
Accuracy: The model's performance was evaluated by checking the probabilities of context words given a center word.

Output Weights: The trained weights for the input-to-hidden and hidden-to-output layers were examined to understand the learned word embeddings.
