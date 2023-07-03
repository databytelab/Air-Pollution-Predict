# Kaggle Tabular Playground Series - Jul 2021 :chart_with_upwards_trend: :trophy:

Welcome to the Kaggle Tabular Playground Series repository! This is a safe space to practice and enhance your ML skills using approachable datasets. This particular project is about predicting air pollution measurements over time based on basic weather information (temperature and humidity) and the readings of five different sensors. 

## 📝 Project Description 

In this project, we are tasked with predicting three air pollution targets: `target_carbon_monoxide`, `target_benzene`, and `target_nitrogen_oxides` based on weather data and sensor readings. The training and test datasets are provided in CSV formats, and a sample submission file is also available to help you format your predictions correctly.

## 📂 Files Description

- `train.csv` - the training dataset, which includes weather data, sensor readings, and values for the 3 target variables.
- `test.csv` - the test dataset, structured similarly to `train.csv`, but without the target values. Your task is to predict these targets.
- `sample_submission.csv` - a sample submission file in the correct format to guide your own submission.

## 📚 Table of Contents

1. [Import Libraries](#import-libraries)
2. [Import Data](#import-data)
3. [Exploratory Data Analysis (EDA)](#eda)
4. [Handle Missing Data](#handle-missing-data)
5. [Encoding Categorical Features](#encoding-categorical-features)
6. [Data Visualization](#data-visualization)
7. [Building the Model](#building-the-model)
8. [Preparing Submission](#eight-preparing-submission-incoming_envelope)

## :one: Import Libraries 

The first step in any machine learning project is importing the necessary libraries. These will depend on the specifics of your project, including the type of data you're working with, the machine learning algorithms you plan to use, etc.

## :two: Import Data 

Once your libraries are imported, the next step is to import your data. In this project, we'll be working with CSV files, which can be easily read into a pandas DataFrame.

## :three: EDA (Exploratory Data Analysis) :mag:

This is where we begin to dive into the data. We'll look for patterns, anomalies, or any relationships that could help us in building our model.

## :four: Handle Missing Data :question:

Handling missing data is crucial for any machine learning project. Depending on the nature of the data and the percentage of data missing, we'll need to decide whether to fill in missing values or to drop those rows/columns entirely.

## :five: Encoding Categorical Features :abc:

Machine learning models require numerical inputs. This step involves transforming categorical features into a suitable numerical form.

## :six: Data Visualization :bar_chart:

Data Visualization is a crucial step in understanding our data. We'll create meaningful plots to understand the relationships between different variables.

## :seven: Building the Model :hammer_and_wrench:

Finally, we get to the heart of the project - building the model. After preparing the data, we can use it to train a model and make our predictions.

## :eight: Preparing Submission :incoming_envelope:

The final step in the process is to prepare our predictions for submission.

Here is a step-by-step guide to get your predictions ready for submission using the `sample_submission.csv`:

1. After building and tuning your model, use it to make predictions on the test dataset.

2. Your predictions will be an array or a list depending on the model and library you used. You should have three separate predictions for `target_carbon_monoxide`, `target_benzene`, and `target_nitrogen_oxides`.

3. Convert your predictions to a pandas DataFrame and ensure it matches the format of the `sample_submission.csv`. Each row should correspond to a row in the test data, and the columns should be in the same order as in `sample_submission.csv`:
    ```
    date_time, target_carbon_monoxide, target_benzene, target_nitrogen_oxides
    ```

4. Save your predictions DataFrame to CSV format. Make sure to exclude the index from your CSV file as it is not required in the submission file.
    ```python
    predictions.to_csv('my_submission.csv', index=False)
    ```
    
5. Now, you're ready to submit your predictions to Kaggle! Navigate to the competition page, click on the "Submit Predictions" button. Then, upload your CSV file and wait for your score.

Remember, you can make up to a certain number of submissions per day, so you have room to experiment and try to improve your score. Good luck! :four_leaf_clover:

