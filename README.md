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
This project explores the application of Deep Reinforcement Learning (DRL) for stock trading. By integrating multiple data sources like raw stock prices, technical indicators, and candlestick charts, the model aims to create a dynamic and adaptive trading strategy to maximize returns and manage risks.

## Project Overview
The system leverages DRL to make automated trading decisions under real-time market conditions. It processes historical market data to learn optimal trading strategies while considering factors such as risk management, market volatility, and transaction costs.

## Key Features
- **Multisource Data Integration**:
  - Raw stock data processing
  - Integration of technical indicators
  - Recognition of candlestick patterns
  - Support for real-time market data feeds

- **Advanced DRL Implementation**:
  - Dueling Deep Q-Network (DQN) architecture
  - Custom reward function incorporating:
    - Sharpe Ratio for risk-adjusted performance
    - Profit Rate for return optimization
    - Transaction cost adjustments

- **Market Analysis Tools**:
  - Evaluation of diverse market conditions
  - Scenarios including growth, decline, and volatile periods
  - Real-time performance tracking and monitoring

## Architecture
```text
Input Layer (State) → Dense Layers → Dueling DQN → Output Layer (Actions)

State Space: Market data, technical indicators, position information
Action Space: Buy, Sell, Hold
Reward Function: Combines Sharpe Ratio and Returns
```

## Results
Performance tested on Apple stock (2015-2022):

| Market Condition | Annualized Return | Sharpe Ratio |
|------------------|-------------------|--------------|
| Volatile Period  | 18.775%          | 0.365        |
| Growth Period    | 0.843%           | 0.063        |
| Decline Period   | -0.927%          | N/A          |

## Technologies Used

**Core Technologies:**
- Python 3.8+
- TensorFlow 2.x
- Keras

**Data Processing:**
- Pandas
- NumPy
- yfinance

**Visualization:**
- Matplotlib
- Seaborn
- Plotly

## Installation

Clone the repository:
```bash
git clone https://github.com/yourusername/Deep-Reinforcement-Learning-Stock-Trading.git
cd Deep-Reinforcement-Learning-Stock-Trading
```

Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Configure your parameters in `config.yaml`:
```yaml
model:
  learning_rate: 0.001
  batch_size: 32
  memory_size: 1000
```

Run the training process:
```bash
python train.py --config config.yaml
```

Evaluate the trained model:
```bash
python evaluate.py --model_path models/best_model.h5
```

## Project Structure
```
├── data/
│   ├── raw/
│   └── processed/
├── models/
│   └── saved_models/
├── notebooks/
│   └── analysis.ipynb
├── src/
│   ├── agents/
│   ├── environment/
│   └── utils/
├── tests/
├── config.yaml
├── requirements.txt
└── README.md
```

## Contributing

1. Fork the repository
2. Create your feature branch:
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [Deep-Q-Trading](https://github.com/Deep-Q-Trading) for inspiration
- [FinRL](https://github.com/AI4Finance-Foundation/FinRL) for market environment design
