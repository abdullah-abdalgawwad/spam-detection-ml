# Spam Comments Detection with Machine Learning

## Overview
This project implements a simple spam comments detection system using Machine Learning. The system classifies YouTube comments as either `Spam` or `Not Spam` based on their content. The model is built using a Naive Bayes classifier and trained on a labeled dataset.

## Features
- Preprocesses and vectorizes text data using CountVectorizer.
- Trains a Bernoulli Naive Bayes model for binary classification.
- Provides predictions for new sample comments.
- Evaluates the model’s performance with accuracy on a test dataset.

## Dataset
The dataset used for this project is `Youtube01-Psy.csv`. It contains YouTube comments with the following columns:
- **CONTENT**: The text of the comment.
- **CLASS**: A binary label where `0` represents `Not Spam` and `1` represents `Spam Comment`.

## Requirements
Make sure you have the following Python libraries installed:

- `pandas`
- `numpy`
- `scikit-learn`

You can install the dependencies using pip:
```bash
pip install pandas numpy scikit-learn
```

## Usage
### Step 1: Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/abdullah-abdalgawwad/spam-detection-ml.git
```

### Step 2: Navigate to the Project Directory
```bash
cd spam-detection-ml
```

### Step 3: Run the Script
Run the Python script to use the model and test sample comments:
```bash
python spam_comments_detection_gui.py
```

### Step 4: Test Sample Comments
The script includes example comments to test the model. You can modify these or add your own samples to see how the model performs.

## GUI Preview

![Screenshot 2024-12-23 083123](https://github.com/user-attachments/assets/0535864e-6ffe-43b3-b5ac-487d3f66049b)

## Code Explanation
### Main Steps:
1. **Data Loading**:
   - Reads the dataset and filters the relevant columns (`CONTENT` and `CLASS`).

2. **Preprocessing**:
   - Converts labels to human-readable values (`Spam Comment`, `Not Spam`).
   - Converts text data to a bag-of-words representation using `CountVectorizer`.

3. **Model Training and Evaluation**:
   - Splits the data into training and testing sets.
   - Trains a Bernoulli Naive Bayes classifier.
   - Evaluates the model’s accuracy on the test set.

4. **Sample Prediction**:
   - Tests the model with predefined sample comments and predicts whether they are spam or not.

### Output:
- Accuracy of the model on the test data.
- Predictions for sample comments.

## Example Output
```text
Model Accuracy: 0.95
Sample Comment: "Check this out: https://thecleverprogrammer.com /"
Prediction: Spam Comment

Sample Comment: "Lack of information!"
Prediction: Not Spam
```

## Enhancements
- Add additional features (e.g., comment length, special characters).
- Experiment with other machine learning models.
- Use a larger and more diverse dataset for better generalization.
- Implement a user interface for real-time predictions.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Author
[Abdullah](https://github.com/abdullah-abdalgawwad)

Feel free to contribute to this project by creating issues or submitting pull requests!

