# Finstreet# 
Algorithmic Trading System - SONATA Stock

Machine learning-based trading strategy using Random Forest for directional prediction of SONATA stock movements.

## 🎯 Overview

- **Model**: Random Forest Classifier (200 trees, depth=6)
- **Strategy**: 5-day forward return prediction (UP/DOWN)
- **Data**: Hourly OHLCV data (Nov-Dec 2025, 280 samples)
- **Features**: 5 technical indicators (returns, SMA, volatility, RSI)

## 📊 Performance

| Metric | Value |
|--------|-------|
| Directional Accuracy | 50.6% |
| Sharpe Ratio | -1.22 |
| Max Drawdown | -2.74% |
| Total Return | -1.59% |

## 🚀 Quick Start

```bash
# Install dependencies
pip install scikit-learn pandas numpy matplotlib seaborn

# Run the notebook
jupyter notebook fin.ipynb
```

## 📁 Project Structure

```
fin.ipynb           # Main analysis notebook
SONATA.csv          # Historical price data
README.md           # This file
```

## 🔧 Key Components

1. **Data Preprocessing**: Clean OHLCV data, engineer features
2. **Feature Engineering**: SMA, RSI, volatility, returns
3. **Model Training**: 70/30 train-test split, standardized features
4. **Backtesting**: Walk-forward validation with risk controls
5. **Risk Management**: 2% stop-loss, 4% take-profit

## ⚠️ Limitations

- Limited dataset (only 2 months)
- No transaction costs modeled
- FYERS API integration not implemented
- Low predictive accuracy
- **NOT PRODUCTION-READY**

## 🔮 Future Improvements

- [ ] Expand dataset to multi-year timeframe
- [ ] Add sentiment analysis features
- [ ] Implement ensemble models (XGBoost, LSTM)
- [ ] Include transaction costs and slippage
- [ ] Complete FYERS API integration
- [ ] Multi-asset portfolio approach

## 📝 License

Educational/Research purposes only. Not financial advice.

## ⚡ Disclaimer

This system is for educational purposes only. Do not use for live trading without significant improvements and proper risk assessment. Past performance does not guarantee future results.
