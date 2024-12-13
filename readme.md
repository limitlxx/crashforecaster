# Time Series Forecasting Web App

## Overview

This is a simple web application that allows users to input numerical data, train a machine learning model, and generate time series forecasts using Brain.js LSTM (Long Short-Term Memory) neural network.

## Features

- Interactive data input
- Local storage of data points
- Real-time visualization of input data
- Machine learning-based time series forecasting
- Color-coded data representation
- Simple and intuitive user interface

## Technologies Used

- HTML5
- Tailwind CSS
- Brain.js (Recurrent Neural Network library)
- JavaScript

## How to Use

1. **Adding Data Points**
   - Enter a number in the input field
   - Click "Add to Array" to store the data point
   - Repeat to build your dataset

2. **Data Visualization**
   - Colored circles represent your input data
   - Color indicates the value:
     - Red: Low values
     - Green: Medium values
     - Yellow: High values
     - Gray: Zero or undefined

3. **Training the Model**
   - Click "Train Model" once you have at least 6 data points
   - The app will normalize your data and train an LSTM neural network
   - A loading indicator will show during training

4. **Forecasting**
   - After training, the app generates 6 forecasted values
   - Forecasted values are displayed with the same color-coding system

5. **Clearing Data**
   - Use the "Clear Storage" button to reset all data

## Technical Details

- Data is normalized before training to improve model performance
- Uses a sliding window approach for time series prediction
- Leverages Brain.js LSTMTimeStep for sequence prediction
- Stores data in browser's localStorage for persistence

## Limitations

- Requires at least 6 data points for training
- Prediction accuracy depends on the quality and quantity of input data
- Best used with consistent, meaningful time series data

## Potential Improvements

- Add data export/import functionality
- Implement more advanced normalization techniques
- Allow customization of neural network parameters
- Add more detailed forecasting visualizations

## Installation

1. Download the HTML file
2. Open directly in a modern web browser
3. No additional setup required

## License

MIT License

## Contributing

Feel free to fork the project and submit pull requests with improvements or bug fixes.