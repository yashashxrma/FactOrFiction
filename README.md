# FactOrFiction - Fake News Detection Model

FactOrFiction is a machine learning-based model designed to detect fake news articles. This README provides an overview of the fake news detection model and its implementation.

## Model Overview

FactOrFiction's fake news detection model is built using a combination of natural language processing techniques and machine learning algorithms. The goal of the model is to classify news articles as either real or fake based on their content.

### Dataset

The model is trained on a labeled dataset of news articles. The dataset contains a collection of articles, each labeled as "REAL" or "FAKE." This labeled data is crucial for the model to learn the patterns and features that distinguish between authentic and fabricated news content.

### Feature Extraction

To transform the textual content into a format that machine learning algorithms can understand, the model employs the **TF-IDF** (Term Frequency-Inverse Document Frequency) technique. TF-IDF assigns numerical values to words based on their frequency in a document relative to their frequency across all documents in the dataset.

### Algorithm

The **Passive Aggressive Classifier** is chosen as the machine learning algorithm for fake news classification. This classifier is particularly suited for online learning scenarios and is capable of making incremental updates to its model.

## Model Training

To train the model:

1. The dataset is preprocessed to clean and prepare the text data.
2. TF-IDF vectors are created to represent each article.
3. The Passive Aggressive Classifier is trained on the TF-IDF vectors and corresponding labels.

## Model Evaluation

The performance of the model is evaluated using standard metrics such as accuracy, precision, recall, and F1-score. The model's ability to correctly classify both real and fake news articles is measured on a separate testing dataset.

## Usage

1. Ensure you have the required dependencies installed: pip install scikit-learn pandas

2. Clone the repository: git clone https://github.com/yourusername/FactOrFiction.git

3. Navigate to the project directory: cd FactOrFiction

4. Run the model script: python model.py

This script loads the dataset, preprocesses the text data, trains the model, and evaluates its performance.

## Contributing

Contributions to enhance and improve the fake news detection model are welcome. If you're interested in contributing, please follow the steps outlined in the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file 
