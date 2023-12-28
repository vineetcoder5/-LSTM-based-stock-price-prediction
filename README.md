# Stock Predictor using Deep Learning
Overview
This project is a stock price prediction system leveraging deep learning techniques. The model is trained on historical stock data sourced from the National Stock Exchange (NSE) website. Key features such as 'HIGH', 'LOW', 'PREV. CLOSE', '52W H', '52W L', and 'No of trades' are utilized for prediction. Additionally, new columns, 'avg' and 'Next_two_days_avg', are introduced to capture average values and predict future trends.

Model Architecture
The deep learning model is implemented using the Keras framework with a carefully crafted architecture. This includes Batch Normalization for input normalization and several dense layers with varying activation functions to capture complex relationships within the data.

Data Preprocessing
Prior to training the model, data preprocessing is performed. A crucial step involves calculating the percentage change between the 'Next_two_days_avg' and 'avg' columns. Based on this change, a binary 'IncreaseDecrease' column is created to signify whether the stock price is expected to increase or not. The threshold for this classification is set at 0.5.

Stock Simulation
The trained model is then applied to simulate stock investment. The simulation assumes an initial investment amount, and for each prediction made by the model, an investment decision is simulated. If the model predicts an increase in stock price, an investment is made, and the balance is updated based on the simulated stock price changes.

How to Use
1. Data Collection
Download historical stock data from the NSE website.
Ensure the dataset includes relevant features such as 'HIGH', 'LOW', 'PREV. CLOSE', '52W H', '52W L', and 'No of trades'.
2. Data Preprocessing
Modify the feature selection and data cleaning as needed in the code.
Ensure proper column names and data types.
3. Model Training
Train the deep learning model using the provided architecture.
Experiment with different hyperparameters for better performance.
4. Simulation
Run the simulation code to observe the investment performance based on the model predictions.
Adjust the investment amount and other parameters as needed.
Contribution Guidelines
Contributions to this project are welcome! If you find any issues or have ideas for improvement, please open an issue or submit a pull request.


Acknowledgments
Special thanks to the National Stock Exchange for providing the historical stock data.
Inspired by the work of researchers and practitioners in the field of stock market prediction.
Feel free to explore and build upon this project. Happy investing!
