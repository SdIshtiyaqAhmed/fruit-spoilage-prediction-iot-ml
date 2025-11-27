# fruit-spoilage-prediction-iot-ml

![Ethical Project](https://img.shields.io/badge/Ethical-Responsible-green)

## Project Overview

This project uses machine learning to predict fruit spoilage by analyzing environmental sensor data—temperature, humidity, light intensity, and CO₂ concentration—collected from an IoT-enabled cold storage system. It aims to help smallholder farmers and supply chain stakeholders proactively manage storage conditions to reduce post-harvest loss and support sustainable agriculture.

## Ethical Considerations

- Designed to promote food security and minimize waste.  
- Avoids harmful or inappropriate content.  
- Supports sustainable agriculture and social welfare.  
- Respects privacy and responsible data usage.  
- Encourages responsible AI and IoT application for societal benefit.

## Dataset

The dataset used in this project is included in this repository as `Dataset.csv`.  
It contains environmental data points collected in a controlled cold storage environment, including fruit type, temperature (°C), relative humidity (%), light intensity (Lux), CO₂ concentration (ppm), and spoilage classification labels (Good/Bad).

Original dataset title:  
**"A Multi-Parameter Dataset for Machine Learning Based Fruit Spoilage Prediction in an IoT-Enabled Cold Storage System"**  
Authors: Nshekanabo Marius, Stanley Mugisha

## Project Workflow

1. Data preprocessing and cleaning  
   - Handling missing values, encoding categorical variables, and normalization  
2. Exploratory data analysis  
   - Visualizing distributions, correlations, and identifying key patterns  
3. Feature engineering and selection  
   - Choosing the most influential features (temperature, humidity, CO₂, light)  
4. Model training and evaluation  
   - Comparing classifiers such as logistic regression, decision trees, and random forests  
   - Hyperparameter tuning and cross-validation  
5. Deployment and validation  
   - Saving the best-performing model for integration with IoT systems  
6. Documentation and sharing of insights  
   - Detailed notebook with code, analysis, and visualizations

## Results

- The Random Forest classifier achieved the best performance with an accuracy of 99.91%.  
- Precision, recall, and F1-score are all approximately 0.9991, indicating excellent balance between false positives and negatives.  
- Confusion matrix analysis shows nearly perfect classification with only one or two misclassifications out of over 2,000 test samples.  
- Feature importance analysis identifies temperature, CO₂, and humidity as key predictors for spoilage risk.  
- The model effectively differentiates between "Good," "Moderate," and "Bad" storage conditions, supporting real-time use in cold storage monitoring.  
- These metrics demonstrate the model’s robustness for deployment in practical cold chain systems, aiding in food preservation and waste reduction.

## Usage Instructions

- Clone this repository to your local machine:  
