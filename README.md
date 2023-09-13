# Low-Level Wind Shear Alert Prediction System Using Deeo Learning

This project aims to predict the occurrence of low-level wind shear at Soekarno Hatta International Airport using machine learning techniques, specifically a Temporal Convolutional Network (TCN). Low-level wind shear, characterized by rapid changes in wind speed and direction over short distances, poses significant challenges and risks to aviation operations, especially during critical phases such as takeoff and landing.

## Dataset

The dataset used for this project is based on observations from Soekarno Hatta International Airport, located in Tangerang, Indonesia.

## Methodology

The project uses a Temporal Convolutional Network (TCN) to predict wind shear occurrences. The model is trained to predict the occurrence of wind shear in the next hour, based on 10-minute data windows sampled every 5 seconds.

## Libraries and Tools

Key Python libraries used in this project include:
- NumPy
- Pandas
- Scikit-learn
- PyTorch
- Plotly
- Matplotlib

The code also uses a function to set a seed for random processes to ensure reproducibility of results.

## Installation

You can install the necessary libraries using either pip or Conda.

For pip, use the requirements.txt file:
```
pip install -r requirements.txt
```



For Conda, use the environment.yml file:
```
conda env create -f environment.yml
```


## Running the Code

After installing the necessary libraries, you can run the following Jupyter notebooks.

* 1-eda.ipynb : visualized and summarized data to gain insights for downstream tasks
* 2-preprocessing.ipynb : linearly interpolated missing data, create input sequences and target variable (binary indicator, 1 if warning in the next 1 hour, 0 otherwise)
* 3-feature engineering.ipynb : created rolling mean and variance features
* 4-results.ipynb : trained TCN and LSTM models and evaluate their performances respect to various metrics and visualized trade off between false positives and false negatives

## Acknowledgements

This analysis was completed as a research project required for a master's degree at the University of Washington.
