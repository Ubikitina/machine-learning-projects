# Project 2: Neural Network Architectures for MNIST Classification

This project investigates the performance of different neural network architectures on the **MNIST handwritten digit classification task**. Using TensorFlow and Keras, the study systematically explores how variations in network depth, the number of neurons, and the learning rate impact model accuracy and loss.

The analysis is structured into four main experiments:
1.  **3-Hidden-Layer Networks:** Various neuron configurations were tested with a fixed learning rate of `3e-1`. The `400-300-300` neuron architecture was identified as the top performer.
2.  **4-Hidden-Layer Networks:** A similar exploration was conducted for deeper networks. The `300-200-200-200` configuration yielded the best results, showing that adding a fourth layer did not provide a significant performance boost over the 3-layer models.
3.  **Learning Rate Tuning (3-Layer Model):** The best 3-layer network was re-evaluated with a new, optimized learning rate of `2e-1`. This adjustment resulted in a marginal improvement in validation and test loss.
4.  **Learning Rate Tuning (4-Layer Model):** The best 4-layer network was tested with an optimized learning rate of `1.5e-1`. The impact on performance was minimal, suggesting the initial learning rate was already effective.

Overall, all tested models achieved high accuracy (over 97%), indicating the MNIST dataset is well-suited for these architectures. The experiments demonstrate that while architectural and hyperparameter adjustments can fine-tune performance, even relatively simple deep learning models can achieve excellent results on this foundational computer vision problem.