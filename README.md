# ANN Classification Project

This project implements an Artificial Neural Network (ANN) for classification tasks using Python. The application is built with Streamlit, providing an interactive web interface for users to interact with the model.

## Project Structure

- `app.py`: Main Streamlit application file
- `model.py`: Contains the ANN model implementation
- `requirements.txt`: Lists all project dependencies
- `experiments.ipynb`: Jupyter notebook containing model development and experimentation

## Experimental Process

### 1. Data Preparation
- Data loading and preprocessing
- Feature scaling and normalization
- Train-test split (typically 80-20 or 70-30)
- Handling missing values and outliers

### 2. Model Architecture
The ANN model is built with the following structure:
- Input Layer: Matches the number of features
- Hidden Layers: 
  - First hidden layer with ReLU activation
  - Second hidden layer with ReLU activation
- Output Layer: Sigmoid activation for binary classification
- Dropout layers for regularization

### 3. Training Process
- Model compilation with appropriate optimizer and loss function
- Batch size and epochs configuration
- Validation split during training
- Early stopping to prevent overfitting
- Learning rate scheduling

### 4. Model Evaluation
- Accuracy metrics calculation
- Confusion matrix analysis
- ROC curve and AUC score
- Cross-validation performance

### 5. Model Optimization
- Hyperparameter tuning
- Architecture adjustments
- Regularization techniques
- Feature selection/engineering

## Features

- Interactive web interface using Streamlit
- Neural network model for classification
- Real-time predictions
- User-friendly data input
- Model performance visualization
- Prediction probability outputs

## Installation

1. Clone this repository
2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Running Locally

To run the application locally, use the following command:
```bash
streamlit run app.py
```

## Deploying to Streamlit.io

Follow these steps to deploy your application to Streamlit.io:

1. Create a GitHub repository and push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin <your-github-repo-url>
   git push -u origin main
   ```

2. Go to [Streamlit.io](https://streamlit.io)
   - Sign up or log in to your account
   - Click on "New app"
   - Connect your GitHub repository
   - Select the repository and branch
   - Set the main file path as `app.py`
   - Click "Deploy"

3. Your app will be deployed and you'll receive a unique URL to access it

## Requirements

The project requires the following Python packages:
- streamlit
- numpy
- pandas
- scikit-learn
- tensorflow (or your preferred deep learning framework)
- matplotlib
- seaborn
- jupyter (for running experiments)

## Usage

1. Open the deployed application
2. Input your data through the web interface
3. The model will process your input and provide predictions
4. View the results directly in the browser