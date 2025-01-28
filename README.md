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




# Deep Reinforcement Learning For Stock Trading

Enhancing Investment Decisions with Deep Reinforcement Learning

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Architecture](#architecture)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction
This project explores the application of deep reinforcement learning (DRL) for stock trading. By integrating multiple data sources like raw stock prices, technical indicators, and candlestick charts, the model aims to create a dynamic and adaptive trading strategy.

## Project Overview
The system uses deep reinforcement learning to make automated trading decisions in real-time market conditions. It processes historical market data to learn optimal trading strategies while considering risk management and transaction costs.

## Key Features
- **Multisource Data Integration**: 
  - Raw stock data processing
  - Technical indicators integration
  - Candlestick pattern recognition
  - Real-time market data feeds

- **Advanced DRL Implementation**:
  - Dueling Deep Q-Network architecture
  - Custom reward function incorporating:
    - Sharpe Ratio for risk assessment
    - Profit Rate for return optimization
    - Transaction cost consideration

- **Market Analysis**:
  - Comprehensive market condition evaluation
  - Support for multiple trading scenarios
  - Real-time performance monitoring
  - Risk management protocols

## Architecture
```text
Input Layer (State) → Dense Layers → Dueling DQN → Output Layer (Actions)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
