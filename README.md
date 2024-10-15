# Requirements for Class Diagram Generation

This repository contains the implementation of our *Requirements to Class Diagram Generation* model. The project focuses on automatically generating class diagrams from natural language requirements using machine learning techniques. Below, you can find information about the requirement problems, dataset, and the code implementation for training and predicting the class diagrams.

## Table of Contents

- [Overview](#overview)
- [How to Use](#how-to-use)
- [Model Training and Prediction](#model-training-and-prediction)
- [Datasets and Models](#datasets-and-models)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project aims to bridge the gap between requirements engineering and class diagram generation by leveraging a machine learning framework. The model takes natural language requirements as input and outputs class diagrams that capture key elements such as classes, attributes, and relationships.

## How to Use

1. Review the dataset in the `Dataset` folder, which contains the requirement problems and their analysis.
2. Use the provided notebooks to train the model and predict class diagrams:
   - The `AutomateRE_model_training.ipynb` notebook is used for model training.
   - The `Predict_results.ipynb` notebook is used for predicting class diagrams using the trained models.
3. Train your own models using the dataset or load the pre-trained models from the `Model` folder to test the prediction functionality.

## Model Training and Prediction

The project includes two main Jupyter notebooks for training the model and making predictions:

1. **AutomateRE_model_training.ipynb**: This notebook is used for training the machine learning model that converts natural language requirements into class diagrams.
   
   - It reads the dataset from the `Dataset` folder and performs preprocessing, model training, and validation.
   
2. **Predict_results.ipynb**: This notebook is used for predicting class diagrams from new natural language requirements.

   - The trained models are loaded from the `Model` folder, and new input requirements are passed through the model to generate class diagrams.

## Datasets and Models

- **Dataset Folder**: Contains the datasets used for training and analyzing the model, including the `Requirements.csv`, `Requirements_ProblemAnalysis.csv`, and `r12_problems.csv` files. The dataset includes 106 requirement problems, detailed textual analysis, and a subset of 12 problems for additional testing.
  
- **Model Folder**: Stores the trained models used in the prediction notebook. These models are generated during the training process and are utilized by the `Predict_results.ipynb` notebook to make predictions on new input requirements.

## Contributing

We welcome contributions to enhance this project! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
