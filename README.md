## **DSCOVRY - Advanced Data Preprocessing and Space Weather Forecasting using DSCOVR Data from L1**

## Overview

DSCOVRY is a project that addresses the critical challenge of near real-time probabilistic plasma flow analysis and weather forecasting using modern machine learning techniques. This project uses space agency open data, including the DSCOVR mission at the Lagrangian point (L1), Kp index, and Dst index, to provide comprehensive insights into space weather conditions.

## Key Features

- **Data Retrieval & Preprocessing:** DSCOVRY accesses and preprocesses data from DSCOVR, Kp, and Dst datasets, ensuring data integrity and readiness for analysis.

- **Linear Interpolation & Data Cleaning:** Our data cleaning process includes linear interpolation for short intervals (5 minutes or less) to handle missing values. Columns with extensive consecutive NaN values (i.e., more than 14 days) are removed from consideration.

- **Machine Learning Model Implementation:** The Neural Network architecture includes Long Short-Term Memory (LSTM) networks and Dense Layers, to forecast plasma flow and geomagnetic storm conditions.

- **Uncertainty Estimation:** Following the methodology described by Tasistro-Hart et al., DSCOVRY aim to provide uncertainty estimates for model output, assisting users in making informed decisions.

- **User-Friendly Interface:** In parallel, we are developing a user-friendly Streamlit app to seamlessly integrate the machine learning model and data visualisation.


## Project Structure

The project structure is organized as follows:

- `dataset/`: Contains data files and datasets.
- `models/`: Stores trained machine learning models.
- `notebooks/`: Jupyter notebooks for data exploration and model development.
- `src/`: Source code for data preprocessing, model implementation, and the Streamlit app.
- `tmp/`: Temporary files and caches used during data retrieval.

## Contributors

- [robotAstray](https://github.com/robotastray)
- [Joseph](https://github.com/3aunuggets)

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/robotAstray/DSCOVR-plasma-analysis/blob/development/LICENSE) file for details.

## Acknowledgments

We would like to acknowledge the DSCOVR, World Data Center for Geomagnetism - Kyoto (WDC Kyoto) open data and resources for space weather analysis.

