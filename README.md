# 📈 Stock Price Prediction GUI

This project is a **Tkinter-based desktop application** that predicts the future closing prices of blue-chip stocks using a pre-trained deep learning model (`finalmodel.h5`). The app allows users to select a stock, input a historical date, and receive predictions for the next 4 days along with a visual chart.

## 🚀 Features

- User-friendly **graphical interface** using Tkinter.
- Predicts stock prices for the next **4 trading days** based on the past 60 days of historical data.
- Visualizes both historical and predicted data on a **matplotlib chart**.
- Uses **Yahoo Finance** (`yfinance`) to fetch real-time stock data.
- Displays prediction results in a **scrollable text box**.

---

## 📦 Requirements

Make sure the following Python packages are installed:

```bash
pip install yfinance numpy pandas scikit-learn matplotlib tensorflow tk tkcalendar
```

---

## 🧠 Pre-requisite

A pre-trained Keras model (`finalmodel.h5`) must be placed in the same directory as the script. This model should take a sequence of 60 normalized prices and predict the next closing price.

---

## 🖥️ Usage

Run the script using Python:

```bash
python stock_predictor_gui.py
```

### Inside the App:
1. Select a stock from the dropdown menu.
2. Choose a date (the last date of the historical range you want to use).
3. Click "Predict" to see the next 4 days' predicted closing prices.
4. The results will be displayed in a scrollable text box.
5. A matplotlib plot will show the past 60 days of actual prices and the next 4 days of predicted prices.

---

## 📊 Supported Stocks

The app currently supports the following **blue-chip** stocks:

- Apple (`AAPL`)
- Microsoft (`MSFT`)
- Amazon (`AMZN`)
- Google (`GOOGL`)
- Tesla (`TSLA`)
- Facebook (`FB`)
- JPMorgan Chase (`JPM`)
- Visa (`V`)
- Johnson & Johnson (`JNJ`)
- Walmart (`WMT`)

---

## 📁 File Structure

```
.
├── stock_predictor_gui.py     # Main Python file with GUI and prediction logic
├── finalmodel.h5              # Pre-trained LSTM or other DL model
├── README.md                  # Documentation file
```


## 💠 Customization

You can modify the list of supported stocks by editing the `BLUE_CHIP_STOCKS` list in the script.

To change the model architecture or training process, retrain a new model and save it as `finalmodel.h5`.

---

## 🧮 Credits

- Developed using **TensorFlow**, **Matplotlib**, **Tkinter**, and **yfinance**.
- Stock data fetched live via the [Yahoo Finance API](https://pypi.org/project/yfinance/).

---

## 📬 Contact

If you have questions or feedback, feel free to open an issue or reach out!

