# Cryptocurrecy Forecasting
Used deep learning networks to forecast movement of cryptocurrency prices. Measured the accuracy of the various architectures using the following pairs:
* Bitcoin (BTC) - Tether (USDT) (used to train the models)
* Ethereum (ETH) - Bitcoin (BTC)
* Litecoin (LTC) - Bitcoin (BTC)

## Results key models

## CNN
| Model                         | ETH-BTC val. | BTC-USDT val.  | LTC-BTC val.  |
|-------------------------------|--------------|----------------|---------------|
| Baseline Model                | 31.0%        | 44.0%          | 46.7%         |
| VGGLike 2, ker. 5             | 37.6%        | 47.3%          | 50.6%         |
| VGGLike 4, ker. 5             | 35.7%        | 46.5%          | 48.5%         |
| VGGLike 8, ker. 5             | 33.3%        | 46.0%          | 43.1%         |
| CNN 2-2-2, ker. 5             | 43.7%        | 56.4%          | 59.0%         |
| CNN 2-2-2, ker.5 (no pooling) | 40.2%        | 52.7%          | 52.7%         |

## RNN
| Model                   | ETH-BTC val.  | BTC-USDT val.  | LTC-BTC val.  |
|-------------------------|---------------|----------------|---------------|
| Baseline Model          | 31.0%         | 44.0%          | 46.7%         |
| RNN 2 layers, 5 hidden  | 36.3%         | 49.8%          | 53.1%         |
| RNN 2 layers, 10 hidden | 34.5%         | 49.0%          | 51.3%         |
| RNN 3 layers, 5 hidden  | 38.4%         | 51.9%          | 53.5%         |
| RNN 3 layers, 10 hidden | 33.7%         | 45.7%          | 49.8%         |
| RNN 4 layers, 10 hidden | 39.5%         | 53.7%          | 56.3%         |
| GRU 3 layers, 5 hidden  | 37.0%         | 49.3%          | 51.9%         |
| LSTM 3 layers, 5 hidden | 32.3%         | 42.9%          | 46.6%         |
