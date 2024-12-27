# Glucose Monitoring System Using Near-Infrared Technology

## Project Overview
This project implements a glucose monitoring system that works without breaking the skin, using Near-Infrared (NIR) Spectroscopy. The system uses an 18-channel NIR sensor to detect glucose levels by analyzing how light is absorbed and reflected at different wavelengths up to 940 nanometers.

## How It Works
The system operates on the principle of NIR spectroscopy:
1. Light is emitted at 18 different wavelengths through the NIR sensor
2. Some light is absorbed by the tissue and glucose molecules
3. Some light is reflected back to the sensor
4. The absorption/reflection patterns at different wavelengths correlate with glucose levels
5. Data is collected every 5 minutes to track glucose variations

## Dataset
- **Input Features**: 18 channels of NIR wavelength data
- **Target Variable**: Continuous Glucose Monitoring (CGM) values
- **Sampling Rate**: Data points collected every 5 minutes
- **Time Period**: Multiple days of readings

## Analysis Pipeline

### 1. Exploratory Data Analysis (EDA)
- Statistical summary of channel readings
- Correlation analysis between channels and CGM values
- Time series analysis of glucose patterns
- Identification of key wavelengths with strong glucose correlations

### 2. Feature Engineering
- Signal preprocessing and noise reduction
- Feature selection based on wavelength importance
- Time-based feature extraction
- Handling missing values and outliers

### 3. Modeling Approaches
Various models are implemented and compared:
- Classical Least Squares (CLS) Calibration
- Partial Least Squares (PLS) Regression
- Support Vector Regression (SVR)
- Neural Networks
- Random Forests
- Ridge Regression

### 4. Evaluation Metrics
- Root Mean Square Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score
- Mean Absolute Percentage Error (MAPE)
- Explained Variance Score

## Technical Implementation
- Python-based analysis using libraries like NumPy, Pandas, Scikit-learn
- Time series analysis tools
- Machine learning models for glucose prediction
- Visualization using Matplotlib and Seaborn

## Key Findings
- Identification of most relevant NIR wavelengths for glucose detection
- Analysis of prediction accuracy across different models
- Understanding of temporal patterns in glucose variations
- Correlation between specific wavelengths and glucose levels

## Future Work
- Model optimization and hyperparameter tuning
- Real-time prediction implementation
- Integration with wearable devices
- Enhanced feature engineering techniques
- Improved accuracy through ensemble methods

## References
1. [New Generation of Sensors for Non-invasive Blood Glucose Monitoring](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10331674/)

