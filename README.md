# RNN Text Generation

## Introduction

This is a simple implementation of a Recurrent Neural Network (RNN) for text generation using PyTorch. The model is trained to predict the next character in a sequence of text, given the previous characters. This README file provides an overview of the code structure, how to use it, and how to train and generate text using the model.

## Requirements

- Python 3.x
- PyTorch
- NumPy

## File Description

- `rnn_text_generation.py`: Main Python script containing the RNN model definition, training loop, and text generation functions.
- `README.md`: This file, containing instructions and information about the project.
- `requirements.txt`: A list of Python dependencies required to run the code.

## Usage

1. Clone the repository:

    ```
    git clone https://github.com/your-username/rnn-text-generation.git
    ```

2. Navigate to the project directory:

    ```
    cd rnn-text-generation
    ```

3. Install dependencies:

    ```
    pip install -r requirements.txt
    ```

4. Train the model:

    ```
    python rnn_text_generation.py train
    ```

5. Generate text using the trained model:

    ```
    python rnn_text_generation.py generate
    ```

## Model Architecture

The RNN model consists of a single RNN layer followed by a fully connected layer. During training, the model takes sequences of one-hot encoded characters as input and predicts the next character in the sequence. The model is trained using cross-entropy loss and optimized using the Adam optimizer.

## Training Data

The training data consists of a list of sentences. Each sentence is treated as a sequence of characters, and the model is trained to predict the next character in each sequence.

## Hyperparameters

- Hidden dimension: 12
- Number of RNN layers: 1
- Learning rate: 0.01
- Number of epochs: 100

You can adjust these hyperparameters in the `rnn_text_generation.py` script according to your requirements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
