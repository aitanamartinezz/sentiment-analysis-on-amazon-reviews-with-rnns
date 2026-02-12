# Sentiment Analysis on Amazon Reviews with RNNs



This project focuses on sentiment classification on the Amazon Reviews dataset using recurrent neural networks (RNNs).

The goal is to evaluate how different RNN architectures and training configurations perform on a real-world NLP task.



The work emphasizes model evaluation, comparison, and practical trade-offs rather than purely architectural novelty.



---



## Problem Context



Sentiment analysis is a common natural language processing task with direct applications in product feedback analysis, customer experience monitoring, and decision support.

User-generated reviews are sequential by nature and often noisy, making them a suitable candidate for sequence models such as RNNs.



In this project, the task is formulated as a supervised binary classification problem:

predicting the sentiment of a review based on its text.



---



## Dataset



The project uses a subset of the \*\*Amazon Reviews\*\* dataset, consisting of text reviews and associated sentiment labels.



Key characteristics:

- Textual, sequential data

- Variable-length inputs

- Binary sentiment labels

- Real-world noise and vocabulary diversity



Text preprocessing includes tokenization, sequence padding, and embedding-based representations.



---



## Methodology



Several recurrent neural network architectures were implemented and compared:



- Simple RNN

- LSTM

- GRU



The experimental setup focuses on:

- Sequence length selection

- Embedding dimensionality

- Batch size and training stability

- Model capacity vs. generalization trade-offs



All models were trained using the same preprocessing pipeline to ensure fair comparison.



---



## Evaluation Strategy



Model performance was evaluated using:

- Accuracy on validation and test sets

- Training and validation loss curves

- Stability across epochs



Special attention was paid to:

- Overfitting behavior

- Convergence speed

- Sensitivity to hyperparameters



This evaluation-oriented approach allows meaningful comparison between architectures beyond a single metric.



---



## Results



Key observations from the experiments:



- Gated architectures (LSTM and GRU) consistently outperformed Simple RNNs.

- GRU models achieved competitive accuracy with fewer parameters and faster convergence.

- Increasing sequence length improved performance up to a point, after which gains diminished.

- Larger embeddings improved expressiveness but increased the risk of overfitting.



Overall, the best-performing models achieved strong classification accuracy while maintaining stable training behavior.



---



## Conclusions



This project demonstrates the practical advantages of gated RNN architectures for sentiment analysis tasks involving noisy, real-world text data.



Beyond raw performance, the experiments highlight the importance of:

- Careful evaluation

- Controlled comparisons

- Understanding trade-offs between model complexity and generalization



The results reinforce why LSTM and GRU models remain strong baselines for sequence modeling tasks.



---



## Project Structure



sentiment-analysis-on-amazon-reviews-with-rnns/

├── notebooks/ # Experiments and analysis

├── src/ # Reusable model and training code

├── results/ # Metrics, plots, and evaluation outputs

├── docs/ # Additional documentation

└── README.md



---



## Tech Stack



- Python

- TensorFlow / Keras

- NumPy, Pandas

- Jupyter Notebooks



---



## Author



Aitana Martínez





