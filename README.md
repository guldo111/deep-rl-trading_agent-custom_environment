# Deep Learning-Based Trading Agent for Cryptocurrency: Performance Analysis and Evaluation

This project focuses on the development and evaluation of a deep learning-based trading agent using the Proximal Policy Optimization (PPO) algorithm. The trading agent is designed to make informed trading decisions in the cryptocurrency market, specifically for Ethereum (ETH), using historical price data with a 1 hour timeframe.

## Project Overview

The main goal of this project is to train a trading agent using deep reinforcement learning techniques and evaluate its performance. The agent utilizes technical indicators such as Simple Moving Average (SMA), Relative Strength Index (RSI), Bollinger Bands (BB), Stochastic Oscillator, Exponential Moving Average (EMA), and Average True Range (ATR) to make trading decisions.

The environment used for training the trading agent is customizable, allowing for the adjustment of parameters such as lookback period, profit target, and symbol, as well as the take profit and stop loss. This flexibility enables experimentation and adaptation to different cryptocurrencies and market conditions.

Additionally, a second model is under development for portfolio management of cryptocurrencies. This model aims to optimize the allocation of investments across multiple cryptocurrencies based on market analysis and risk management strategies.

The project follows these key steps:

1. Data Preprocessing: The historical price data of Ethereum is loaded from a CSV file and undergoes preprocessing. Technical indicators are calculated and added to the dataset.

2. Train set and Test set: The dataset is divided into train and test set (80% train and 20% test). It is possible to implement a K-fold Cross-Validation.

3. Training and Evaluation Loop: A custom TradingEnvironment is created and transformed into a vectorized environment. The PPO model is then trained on the training environment using the PPO algorithm. The trained model is evaluated on the validation environment.

4. Test Results Saving: The test results including date, prices, volume, technical indicators, actions taken by the agent, stop-loss levels, take-profit levels, and balance, are saved in separate CSV files for further analysis.

## Expected Results

The expected outcomes of this project are:

- The trained PPO model will learn to make trading decisions based on historical price data and calculated technical indicators.

- The test results for each fold will provide insights into the performance of the trading agent, including the actions taken, stop-loss and take-profit levels, and the final account balance.

By analyzing the test results, we can evaluate the effectiveness of the trained trading agent and gain insights into its performance in different market conditions.


## Requirements

The project requires the following dependencies:

- Python 3.7 or above 
- Gym
- Stable Baselines3
- Pandas
- NumPy
- Matplotlib
- mplfinance

To install the dependencies, use pip


## Usage

1. Create a crypto_data folder in your working directory

1. Prepare the historical price data for Ethereum in the `crypto_data` folder.

2. Run the Jupyter Notebook

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## References

If you use this work, please cite:
- Repository: (https://github.com/guldo111/deep-rl-trading_agent-custom_environment/tree/main)
- Author: guldo111

References:
- Gym: [https://gym.openai.com/]
- Stable Baselines3: [https://stable-baselines3.readthedocs.io/]
- mplfinance: [https://github.com/matplotlib/mplfinance]


