# Weather Crop Planning

This project aims to develop a localized weather-informed crop planning system for sustainable agriculture in India. The system integrates weather forecasting and crop recommendation to help farmers make informed decisions about crop selection and cultivation practices. Here's an overview of the key components:

Weather Forecasting Model

The weather forecasting model uses historical weather data from the India Meteorological Department (IMD) to predict weather patterns for the next 90 days in specific districts of Maharashtra. The process involves:

1. Data preprocessing to handle missing values and create new insightful attributes
2. Feature extraction to identify the most relevant weather parameters
3. Implementation of a Long Short-Term Memory (LSTM) neural network model with two layers and ReLU activation
4. Model optimization using Adam optimizer and Mean Squared Error loss function

The model achieves accurate 90-day weather forecasts for the chosen district.

Crop Recommendation Model

This model analyzes crop data from IMD's Agromet dataset to recommend suitable crops based on forecasted weather conditions. Key steps include:

1. Data preprocessing to handle missing values and class imbalance using SMOTE
2. Feature extraction to identify significant crop attributes
3. Implementation of an ensemble model combining Random Forest and AdaBoost classifiers
4. Integration with the weather forecasting model to suggest crops for the 90-day forecast period

The ensemble approach improves the model's accuracy to 95%, overcoming initial challenges with data limitations and class disparities.
