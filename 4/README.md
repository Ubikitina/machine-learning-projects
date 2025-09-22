# Project 4: Face Classification with SVM and Dimensionality Reduction

This project investigates the effectiveness of dimensionality reduction techniques, **Principal Component Analysis (PCA)** and **Linear Discriminant Analysis (LDA)**, when combined with Support Vector Machine (SVM) classifiers for a face recognition task. The analysis is performed on the **Olivetti Faces dataset**.

The primary goal is to compare the performance of two SVM models, `LinearSVC` and `SVC` (with an RBF kernel), across three different data representations:
1.  The original, high-dimensional image data.
2.  Data compressed with **PCA** to retain 95% of the variance.
3.  Data transformed with **LDA** to maximize class separability.

### Key Experiments and Findings:

* **Dimensionality Reduction:** PCA reduced the feature space from 4096 to 144 components, while LDA, being a supervised method, reduced it to 39 components (one less than the number of classes).

* **Hyperparameter Tuning:** `GridSearchCV` was systematically used to find the optimal hyperparameters (`C` for `LinearSVC`; `C` and `gamma` for `SVC`) for each model and dataset combination.

* **Performance Comparison:**
    * **Accuracy:** The models trained on **LDA-transformed data achieved perfect (100%) accuracy** on the test set, significantly outperforming those trained on original or PCA-reduced data. This highlights LDA's strength in finding a feature space that is highly optimized for classification.
    * **Execution Time:** Both PCA and LDA dramatically reduced the model training time compared to using the original data. The most significant speed-up was observed with LDA, due to it producing the lowest-dimensional dataset.
    * **Model Choice:** While `LinearSVC` generally provided slightly higher accuracy on the original and PCA data, `SVC` was consistently faster to train. On the superior LDA-transformed data, both models reached maximum performance, making either a viable choice.

In conclusion, the study demonstrates that applying a supervised dimensionality reduction technique like LDA is exceptionally effective for this face classification task, leading to both a substantial increase in accuracy and a dramatic reduction in computational cost.