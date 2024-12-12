# Dengue Risk Detection and Observation System

## Project Overview

The Dengue Risk Detection and Observation System is an advanced AI-driven tool developed in collaboration with the Tainan City Government to predict and monitor dengue fever outbreaks. Leveraging cutting-edge models, such as Graph WaveNet (GWNet) and XGBoost, the system forecasts mosquito egg counts and positivity rates to identify high-risk areas and assist in effective epidemic prevention measures.

## Key Features

- **Spatio-temporal Analysis**: Combines regional adjacency and temporal correlations to enhance prediction accuracy.
- **User-Friendly Interface**: Interactive visualization tools to explore dengue risk areas and trends.
- **Integration of Multiple Data Sources**:
  - Weather data (temperature, humidity, precipitation, pressure).
  - Ovitrap monitoring data (egg counts and positivity rates).

## Methodology

1. **Data Collection and Preprocessing**:

   - Collected ovitrap data and weather information for Tainan City.
   - Preprocessed and normalized data to reduce skewness and outliers.

2. **Model Implementation**:

   - **GWNet** for total egg count predictions, capturing spatial and temporal features.
   - **XGBoost** for positivity rate predictions, leveraging its ability to handle high-dimensional datasets.

3. **Model Evaluation**:

   - Employed Root Mean Square Error (RMSE) to compare model performance.
   - Conducted cross-validation and hyperparameter tuning for optimization.

4. **System Features**:

   - Interactive risk maps for identifying high, medium, and low-risk areas.
   - Trend visualization for total egg counts and positivity rates.

## Results

### Model Performance

| Model               | RMSE (ln Total Egg Count) | RMSE (Positivity Rate) |
| ------------------- | ------------------------- | ---------------------- |
| Guess Zero          | 7.5248                    | 28.5899                |
| Guess Last Week     | 0.5343                    | 8.7386                 |
| Bayesian            | 0.4878                    | 7.6518                 |
| Linear              | 0.4882                    | 7.6523                 |
| Ridge               | 0.4853                    | 7.6503                 |
| Lasso               | 0.4842                    | 7.6353                 |
| Cross Decomposition | 0.4872                    | 7.6496                 |
| Elastic Net         | 0.4834                    | 7.652                  |
| SVM                 | 0.4818                    | 7.2658                 |
| XGBoost             | 0.4746                    | 7.0071                 |
| LSTM                | 0.5253                    | 8.4432                 |
| GWNet               | 0.4146                    | 7.5811                 |

- **GWNet** achieved the best performance for predicting total egg counts due to its ability to model spatial and temporal relationships.
- **XGBoost** excelled at predicting positivity rates, effectively capturing complex non-linear patterns.


## Web Demo Video

[![](https://img.youtube.com/vi/VzJXCywGHZw/0.jpg)](https://www.youtube.com/watch?v=VzJXCywGHZw)

## Installation and Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/dengue-risk-detection.git


## Future Work

- Integration of additional data sources for enhanced accuracy.
- Expansion to other dengue-prone regions.
- Optimization using advanced AI models.

## Acknowledgments

This project was supported by the National Science and Technology Council (NSTC) under grants [111-2636-E-006-026], [112-2221-E-006-100], and [112-2221-E-006-150-MY3].

## Authors

This project was developed by a research team at National Cheng Kung University in collaboration with the Tainan City Government. 

## References

For detailed references, please refer to the published paper: *Dengue Risk Detection and Observation System* presented at ICKII 2024.



