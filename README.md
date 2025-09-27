# Machine Learning Course Projects

This repository contains the practical assignments developed during the 2024-2025 academic year for the **Machine Learning I** (Aprendizaje Automático I) course, part of the **Master's Degree in Data Science & Engineering** at **UNED**.

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


## License

This project is released under the terms of the **MIT License**.

The purpose of this license is to allow the free reuse of the code for any purpose, provided that the original copyright notice and the license text are included in any copy or substantial portion of the software.[1] This means that while you can use, modify, and distribute this code, **you have a legal obligation to provide original authorship attribution**.

You can find a complete copy of the license text in the `LICENSE` file in this repository.


## Waring on Academic Integrity and Plagiarism

This repository and its contents are published for a dual purpose:

1.  **Educational:** As reference and consultation material for other developers interested in the topics covered.
2.  **Professional:** As part of my personal portfolio to demonstrate my skills and the projects I have worked on.


**⚠️ IMPROPER USE AND CONSEQUENCES:**

The use, copy, or adaptation, in whole or in part, of this work to be submitted as one's own in any course, subject, or academic context—whether at UNED or any other educational institution—constitutes **plagiarism**.

Plagiarism is a **serious offense** against academic integrity, punishable under Universities Academic Disciplinary Regulations and other similar rules. The plagiarism detection tools used by the universities compare student submissions against billions of internet sources, including public GitHub repositories, so any copy will be detected.

By publishing this work under a license that requires attribution, this repository promotes good faith and ethical use of the code. Anyone who ignores the terms of the license and academic regulations to commit fraud does so at their own sole and exclusive risk.