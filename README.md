# Deep Reinforcement Learning For Stock Trading
Enhancing Investment Decisions with Deep Reinforcement Learning

## Introduction
This project explores the application of deep reinforcement learning (DRL) for stock trading. By integrating multiple data sources like raw stock prices, technical indicators, and candlestick charts, the model aims to create a dynamic and adaptive trading strategy.

## Key Features
- **Multisource Data Integration**: The model uses raw stock data, technical indicators, and candlestick charts for a comprehensive market view.
- **Dueling Deep Q-Network**: Implementation of a Dueling Deep Q-Network with a custom reward function balancing risk (Sharpe Ratio) and return (Profit Rate).
- **Market Segment Analysis**: The model is evaluated across different market conditions, including volatile, growth, and decline periods.

## Results
The model was tested on Apple stock data from 2015-2022:
- **Volatile Period**: Achieved an Annualized Return (AR) of 118.775% with a Sharpe Ratio of 0.365.
- **Growth Period**: AR of 0.843%, Sharpe Ratio of 0.063.
- **Decline Period**: Faced challenges with a negative AR of -0.927%.

## Technologies Used
- **Python**: Core programming language.
- **TensorFlow/Keras**: For building and training the neural networks.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib/Seaborn**: For data visualization.

## How to Run the Project
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/Deep-Reinforcement-Learning-Stock-Trading.git
    cd Deep-Reinforcement-Learning-Stock-Trading
    ```
2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter Notebook:
    ```bash
    DRL-Stock-Trading.ipynb
    ```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
