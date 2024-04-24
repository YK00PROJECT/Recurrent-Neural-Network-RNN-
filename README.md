# RNN for Stock Trend Prediction

## Overview
This project develops a Recurrent Neural Network (RNN) designed to predict stock market trends using historical data. The implementation focuses on Google's stock prices, employing Long Short-Term Memory (LSTM) layers within the RNN to capture temporal dependencies and dynamics in stock price movements.

## Repository Structure
- **Google_Stock_Price_Train.csv:** Training dataset containing historical stock price data.
- **Google_Stock_Price_Test.csv:** Test dataset for evaluating the model's performance.
- **stock_rnn.ipynb:** Jupyter notebook containing the full code for the project.

## Installation
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/stock-trend-prediction-rnn.git
   cd stock-trend-prediction-rnn
   ```

2. **Set Up Environment:**
   Ensure Python 3.x is installed and set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

## Usage
Open the `stock_rnn.ipynb` notebook to view and run the step-by-step process for training and evaluating the RNN model. The notebook includes:
- Data Preprocessing: Feature scaling and data transformation to prepare the input for the RNN.
- Model Building: Constructing the LSTM model using Keras.
- Training: Training the model on the dataset.
- Prediction: Making predictions and comparing them to the real stock prices.

## Model Details
The RNN model includes multiple LSTM layers with dropout regularization to prevent overfitting. The model's architecture is as follows:
- LSTM layer with 50 units and return sequences enabled.
- Dropout layer with a 20% dropout rate.
- Three additional LSTM layers with similar configurations.
- A Dense output layer to predict the stock price.

## Results
The model's predictions are visualized against the actual stock prices to assess performance. The notebook includes a plot that demonstrates the model's prediction accuracy on the test set.

## Contributing
Contributions to this project are welcome! If you have improvements or bug fixes, please fork this repository, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Conclusion
This RNN implementation demonstrates the capability of LSTM networks to predict financial market trends accurately. The project serves as a foundational approach to more complex financial predictions using deep learning.

## Visualization
The final section of the notebook includes a matplotlib visualization that plots both the real and predicted stock prices, providing a clear visual comparison of the model's performance.

By following this README, users can replicate the project environment, retrain the model, and potentially improve or adapt the model for other types of time series predictions.
