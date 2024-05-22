# Service Desk Ticket Classification with Deep Learning

## Project Description

Efficient handling of customer service desk tickets is crucial to ensure customer satisfaction. By leveraging deep learning, you will develop a robust and accurate classifier that can categorize incoming service desk tickets into predefined categories, streamlining service desk operations.

## Table of Contents

- [Project Description](#project-description)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Model Building](#model-building)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before starting, ensure you have the following:

- Basic understanding of Python programming and deep learning libraries (e.g., PyTorch).
- Familiarity with text processing and classification tasks.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/service-desk-ticket-classification.git
    cd service-desk-ticket-classification
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Dataset

The dataset used for this project contains service desk tickets and their respective categories. The dataset includes text data representing the ticket content and labels for the predefined categories.

## Data Preparation

1. **Load Data:** Load the dataset using pandas and JSON.
2. **Tokenization:** Tokenize the text data using NLTK.
3. **Mapping:** Create word-to-index and index-to-word mappings.
4. **Padding:** Pad the tokenized text data to a fixed sequence length.

## Model Building

1. **Define Model:** Define a CNN-based model with an embedding layer, convolutional layer, pooling layer, and fully connected layer.
2. **Parameters:** Set parameters such as vocabulary size, embedding dimension, number of classes, and sequence length.

## Model Training

1. **DataLoader:** Create DataLoaders for training and testing datasets.
2. **Loss and Optimizer:** Define the loss function and optimizer.
3. **Training Loop:** Implement the training loop to train the model over several epochs.

## Model Evaluation

1. **Evaluation Function:** Implement a function to evaluate the model on the test dataset.
2. **Metrics:** Calculate accuracy, precision, and recall using `torchmetrics`.

## Usage

To use the trained model for classifying new service desk tickets, follow the instructions provided in the notebook `service_desk_ticket_classification_notebook.ipynb`.

1. **Load Model:** Load the trained model.
2. **Input Data:** Provide the new ticket text as input to the model.
3. **Predict Category:** Generate predictions for the ticket category.

## Results

Document the results of your model, including the evaluation metrics and any visualizations that help interpret the model's performance.

## Contributing

Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are reviewed on a regular basis.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
