# Predicting Life Insurance Liquidity Risk

This project aims to predict the liquidity risk of life insurance using deep learning algorithms: CNN, MLP, LSTM, and RNN. The predictions are made for both insurance sales and claims data from [1397] to [1399] (Gregorian Calendar) or 2018 to 2023. The liquidity risk is calculated by dividing the sales amounts by the claims amounts.

## Table of Contents

1. [Introduction](#introduction)
2. [Data](#data)
3. [Models](#models)
4. [Results](#results)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction

This project focuses on predicting the liquidity risk of life insurance using various deep learning models. The objective is to forecast sales and claims data using CNN, MLP, LSTM, and RNN, and then compute the liquidity risk from these predictions.

## Data

The data used in this project includes:

- **Sales Data**: Insurance sales data from [1397] to [1399] (Gregorian Calendar) or 2018 to 2023.
- **Claims Data**: Insurance claims data from [1397] to [1399] (Gregorian Calendar) or 2018 to 2023.

### Sample Data

Here are the first ten rows of the sales and claims data:

#### Sales Data
![Sales Data](path/to/sales_data_image.png)

#### Claims Data
![Claims Data](path/to/claims_data_image.png)

## Models

We use the following deep learning models for prediction:

1. **Convolutional Neural Network (CNN)**
2. **Multi-Layer Perceptron (MLP)**
3. **Long Short-Term Memory (LSTM)**
4. **Recurrent Neural Network (RNN)**

Each model is trained separately on both sales and claims data.

## Results

The liquidity risk is calculated by dividing the predicted sales by the predicted claims. The results are then evaluated to determine the accuracy and reliability of each model.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/insurance-liquidity-risk-deep-models.git
    ```
2. Navigate to the project directory:
    ```sh
    cd insurance-liquidity-risk-deep-models
    ```
3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Prepare your dataset and place it in the `data` directory.
2. Run the preprocessing script:
    ```sh
    python preprocessing/preprocess_data.py
    ```
3. Train the models for sales:
    ```sh
    python lstm/train_lstm_sales.py
    python cnn/train_cnn_sales.py
    python mlp/train_mlp_sales.py
    python rnn/train_rnn_sales.py
    ```
4. Train the models for claims:
    ```sh
    python lstm/train_lstm_claims.py
    python cnn/train_cnn_claims.py
    python mlp/train_mlp_claims.py
    python rnn/train_rnn_claims.py
    ```
5. Evaluate the models:
    ```sh
    python lstm/evaluate_lstm.py
    python cnn/evaluate_cnn.py
    python mlp/evaluate_mlp.py
    python rnn/evaluate_rnn.py
    ```
6. Visualize the results:
    ```sh
    python visualization/visualize_results.py
    ```

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
