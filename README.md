# Q-A_model_using_RNN

This project demonstrates a basic implementation of a Recurrent Neural Network (RNN) in PyTorch for a simple Question Answering task. The model is trained on a small dataset of unique question-answer pairs to predict answers based on the question text.

**Important Note:** This model is a simplified example designed to predict a *single token* as the answer. It will not correctly generate multi-word answers from the dataset. A more advanced sequence-to-sequence model architecture (like an Encoder-Decoder with LSTMs or Transformers) is required for generating multi-word responses.

## Dataset

The model uses a dataset from `100_Unique_QA_Dataset.csv`, which contains a list of simple questions and their corresponding answers. Ensure this CSV file is available when running the script.

## Features

-   Loads data from a CSV file.
-   Builds a vocabulary of unique tokens from the questions and answers.
-   Converts text data into numerical sequences using the vocabulary.
-   Implements a basic RNN model with an embedding layer.
-   Trains the model using Cross Entropy Loss.
-   Includes a function to predict an answer for a given question.

## Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/rishu1947-ops/Q-A_model_using_RNN
    cd rnn-question-answering # Or whatever you name your repository
    ```

2.  **Obtain the dataset:**
    Make sure the `100_Unique_QA_Dataset.csv` file is present in the project directory. You might need to download it separately if it's not included in the repository.

3.  **Install dependencies:**
    It's recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```
    *Note: Ensure you have the correct PyTorch version installed. Refer to the [PyTorch website](https://pytorch.org/get-started/locally/) for detailed installation instructions.*
