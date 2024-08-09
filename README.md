# Sequence Summation Task with RNNs

This project involves training different Recurrent Neural Networks (RNNs) – Elman Network, Long Short-Term Memory (LSTM), and Gated Recurrent Unit (GRU) – to solve a specific sequence summation task. The performance of these networks is compared against a simple baseline model.

## Task Overview

### Objective:
Given a dataset where each sample is a sequence of variable length and a constant depth of 2, the task is to predict the sum of certain values in the sequence. The sequences are structured as follows:

- The first dimension of the sequence consists of random values within the range [0, 1].
- The second dimension is binary, containing zeros with exactly two elements marked by 1.

The goal is to accurately sum the random values corresponding to the indices where the second dimension has a value of 1.

### Dataset:
- **Variable Length:** Sequences vary in length.
- **Constant Depth:** Depth of 2 for all sequences.
- **First Dimension:** Contains random values in [0, 1].
- **Second Dimension:** Binary values, with exactly two elements marked as 1.

### Models Trained:
1. **Elman Network**
2. **Long Short-Term Memory (LSTM)**
3. **Gated Recurrent Unit (GRU)**

### Baseline Model:
A simple baseline model is used, which always predicts a sum of 1, irrespective of the input sequence.

## Performance Comparison

### Evaluation:
The models were evaluated based on their ability to correctly predict the sum of the values marked by 1. The performance of each RNN was compared against the baseline.

### Results:
- **Loss Order:** The loss values observed during training and evaluation followed this order: Elman Network > LSTM > GRU.
- **LSTM vs. GRU:** Depending on the dataset, LSTM and GRU showed similar performance, often closely matched, with GRU generally performing slightly better.
- **Learning Curves:** Plotted to show the convergence and learning process of each RNN.
- **Final Performance:** Quantitative metrics were used to compare the accuracy and efficiency of each RNN model relative to the baseline.

## Conclusion
This comparison highlights the performance differences between various RNN architectures for sequence-based tasks, showing that while the Elman Network lags behind, LSTM and GRU often perform closely, with GRU typically holding a slight advantage.
