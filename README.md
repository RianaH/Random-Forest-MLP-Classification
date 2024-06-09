# Dry Bean Classification with Random Forest and MLP

This project aims to classify dry beans into different classes using machine learning techniques. It includes data preprocessing, model training, and performance evaluation using Random Forest and Multi-Layer Perceptron (MLP) models.

## Dataset

The dataset used in this project is the Dry Bean Dataset from the UCI Machine Learning Repository. The dataset contains images of 13,611 grains of 7 different registered dry beans, with a total of 16 features extracted from these images.

- **Number of Instances**: 13,611
- **Number of Features**: 16
- **Classes**: 7 (Seker, Barbunya, Bombay, Cali, Dermosan, Horoz, and Sira)

## Features

1. Area
2. Perimeter
3. MajorAxisLength
4. MinorAxisLength
5. AspectRatio
6. Eccentricity
7. ConvexArea
8. EquivDiameter
9. Extent
10. Solidity
11. Roundness
12. Compactness
13. ShapeFactor1
14. ShapeFactor2
15. ShapeFactor3
16. ShapeFactor4

## Setup

To set up the project, follow these steps:

1. Clone the repository:
```bash
git clone https://github.com/RianaH/Random-Forest-MLP-Classification.git
```

3. Navigate to the project directory:
```bash
cd Random-Forest-MLP-Classification
```

4. Create a virtual environment and activate it:
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\\Scripts\\activate`
```

5. Install the required packages:
```bash
pip install -U ucimlrepo
pip install pandas scikit-learn matplotlib torch numpy
```

## Usage

### Data Preprocessing

The data preprocessing steps include:
- Loading the dataset
- Splitting the dataset into training, validation, and test sets
- Scaling the features
- Encoding the labels

### Model Training

#### Random Forest

The Random Forest model is trained using GridSearchCV to find the best hyperparameters. The model's performance is evaluated using accuracy, confusion matrix, ROC curve, and feature importance.

#### Multi-Layer Perceptron (MLP)

The MLP model is defined using PyTorch. The model is trained and validated over multiple epochs, and the loss curves are plotted to monitor the training process. The model's performance is evaluated using accuracy, confusion matrix, and ROC curve.

### Evaluation

Both models are evaluated using:
- Accuracy
- Confusion Matrix
- ROC Curve
- Feature Importance (for Random Forest)

## Visualizations

The project includes various visualizations such as:
- Pair plots of the features
- Class distribution
- Training and validation loss curves
- Confusion matrices
- ROC curves
- Feature importance plots

## Acknowledgements

The dataset was provided by the UCI Machine Learning Repository. Special thanks to the creators of the Dry Bean Dataset.

## License

This project is licensed under the MIT License.
