# fruit-spoilage-prediction-iot-ml

![Ethical Project](https://img.shields.io/badge/Ethical-Responsible-green)

## Project Overview

This project develops a machine learning model to predict fruit spoilage by analyzing environmental sensor data—temperature, humidity, light intensity, and CO₂ concentration—collected from an IoT-enabled cold storage system. The model targets improving post-harvest management for smallholder farmers and supply chain stakeholders, helping reduce food loss and supporting sustainable agriculture.

## Ethical Considerations

- Designed to promote food security and minimize waste.  
- Free from harmful or inappropriate content.  
- Aligns with sustainable agricultural practices and community welfare.  
- Respects data privacy and responsible usage principles.  
- Advocates for responsible deployment of AI and IoT technologies with societal benefit.

## Dataset

This repository includes the dataset as `Dataset.csv`. It consists of environmental data from a controlled cold storage environment, covering four fruit types but with focused modeling on three:

- Fruit types: Orange, Pineapple, Tomato  
- Features: Temperature (°C), Relative Humidity (%), Light Intensity (Lux), CO₂ Concentration (ppm)  
- Label: Spoilage classification with classes like Good, Moderate, and Bad

*Note:* Banana samples exist in the dataset but were not explicitly modeled due to preprocessing steps (one-hot encoding with dropped baseline), so the current model focuses on the three fruits above.

Original dataset title and authors:  
**"A Multi-Parameter Dataset for Machine Learning Based Fruit Spoilage Prediction in an IoT-Enabled Cold Storage System"**  
Nshekanabo Marius, Stanley Mugisha

## Project Workflow

1. Data preprocessing and cleaning  
   - Handle missing data, encode categorical variables, normalize features.  
2. Exploratory data analysis (EDA)  
   - Visualize distributions, identify correlations and outliers.  
3. Feature engineering and selection  
   - Select key predictors like temperature, CO₂, humidity, and light.  
4. Model training and evaluation  
   - Compare classifiers including logistic regression, decision trees, random forests, and gradient boosting.  
   - Tune hyperparameters; validate through cross-validation.  
5. Model deployment preparation  
   - Serialize the best-performing model (`fruit_spoilage_model.joblib`) for integration in IoT systems.  
6. Documentation and sharing  
   - Provide detailed notebook with implementation, results, and insights.

## Results

- The Random Forest classifier achieves outstanding results:  
  - Accuracy: 99.91%  
  - Precision, Recall, F1-score: ~0.9991 each, demonstrating balanced, robust classification.  
- The confusion matrix reveals near-perfect classification across over 2,000 test samples, with minimal misclassifications.  
- Feature importance analysis identifies temperature, CO₂, and humidity as critical for spoilage prediction.  
- The model effectively differentiates storage conditions into "Good," "Moderate," and "Bad," enabling actionable insights for cold storage monitoring.  
- This performance supports practical deployment to support food preservation and reduce waste for targeted fruit types.

## Usage Instructions

- Clone this repository:  
git clone https://github.com/SdIshtiyaqAhmed/fruit-spoilage-prediction-iot-ml.git
- Use the included `Dataset.csv` file for data and model training.  
- Explore and run the step-by-step instructions in the `fruit_spoilage_prediction_iot_ml.ipynb` notebook to replicate preprocessing, modeling, evaluation, and visualization.  
- The trained machine learning model is saved as `fruit_spoilage_model.joblib` for inference or integration.  

## Acknowledgments

This project’s code and documentation were generated using Google Colab’s Gemini AI feature.  
Thanks to Nshekanabo Marius and Stanley Mugisha for the dataset that enables this work.

## License

This project is licensed under the MIT License.

---

Promoting sustainable food preservation and the ethical use of technology to create social impact.
