# Machine Learning Course Projects

This repository contains the practical assignments for the **Machine Learning I** (Aprendizaje Automático I) course, part of the **Master's Degree in Data Science & Engineering** at **UNED**.

The purpose of this repository is to store and document the projects developed during the course, using popular machine learning tools and frameworks like **scikit-learn**, **Keras**, and **TensorFlow**.

## Repository Structure

This repository contains a collection of four machine learning projects. Each project is self-contained in its own directory and includes a detailed `README.md` with summarizing the analysis, findings, and code.


- [Project 1: Foundational Models on Airbnb Data](./1/)

  - **Objective:** Classify Airbnb room types in Madrid.
  - This project serves as an introduction to fundamental classification algorithms. It involves a deep dive into data cleaning, exploratory data analysis (EDA), and the implementation of **Naive Bayes**, **K-NN**, and **Decision Trees** to predict listing categories.

- [Project 2: Neural Networks for Image Recognition](./2/)

  - **Objective:** Classify handwritten digits from the MNIST dataset.
  - A practical exercise in deep learning, this project focuses on designing, training, and optimizing **Neural Networks** with 3 and 4 hidden layers using **TensorFlow** and **Keras**. The impact of network architecture and learning rates is systematically evaluated.


- [Project 3: Support Vector Machines for Classification & Regression](./3/)

  - **Objective:** Predict Airbnb room types and prices.
  - Revisiting the Airbnb dataset, this project explores the versatility of **Support Vector Machines (SVMs)**. It tackles both a classification problem (predicting `room_type` with `SVC`) and a regression challenge (predicting `price` with `SVR`), including extensive hyperparameter tuning.


- [Project 4: Dimensionality Reduction for Face Recognition](./4/)

  - **Objective:** Classify faces from the Olivetti Faces dataset.
  - This project showcases advanced techniques by combining SVMs with dimensionality reduction. It provides a comparative analysis of **PCA (unsupervised)** and **LDA (supervised)** to see how they impact classification accuracy and computational efficiency in a high-dimensional feature space.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

The projects are developed using **Jupyter Notebooks** (`.ipynb`) and require a Python environment. This guide uses **conda** for environment management.

  - Python 3.9
  - conda

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/machine-learning-projects.git
    cd machine-learning-projects
    ```

2.  **Create and activate the conda environment:**
    A new environment named `machine_learning` will be created with all the necessary dependencies.

    ```bash
    conda create -n machine_learning python=3.9 scikit-learn keras tensorflow jupyter -y
    conda activate machine_learning
    ```

3.  **Launch Jupyter Notebook:**
    Once the environment is activated, you can run the notebooks.

    ```bash
    jupyter notebook
    ```

## Contributing

Suggestions, improvements, or corrections are highly welcome. Please feel free to open a **pull request**, and I will be glad to review it.
