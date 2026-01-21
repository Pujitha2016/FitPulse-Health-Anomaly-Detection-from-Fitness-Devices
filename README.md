FitPulse-Health-Anomaly-Detection-from-Fitness-Devices

Overview:

This project focuses on analyzing time-series health data generated from fitness watch devices such as Fitbit, Apple Watch, and other wearables. These devices continuously record biometric data including heart rate, sleep duration, step count, and physical activity levels. Although this data contains valuable insights, users and healthcare professionals often overlook subtle early signs of health anomalies. This system applies anomaly detection techniques to automatically flag unusual health patterns and supports personalized preventative healthcare.


Objective:

The primary objective of this project is to detect anomalies in wearable health data and present diagnostic insights through a dashboard. The project is designed to support data-driven decision making for improving lifestyle, identifying irregular health events, and monitoring overall wellness metrics.

FitPulse Health Anomaly Detecti…

Key Features:

Imports fitness tracking data from CSV and JSON files.

Cleans and preprocesses inconsistent time-series data.

Extracts statistical and trend-based time-series features.

Utilizes forecasting models and clustering methods for anomaly identification.

Detects anomalies based on threshold violations, model residuals, and outlier clusters.

Provides a dashboard for visualizing health trends and anomaly insights.

Supports file uploads, filtering by metric, and exporting reports.



Target Outcomes:

The project aims to achieve the following outcomes:

Detect anomalies in heart rate, sleep data, and step count.

Generate personalized health alerts using time-series and clustering techniques.

Provide real-time or batch anomaly detection support.

Allow configurable metric thresholds such as heart rate limits.

Enable interactive visualization of trends and anomalies.

Allow exporting reports for clinical or personal usage.


Modules Implemented:

Module 1: Data Collection and Preprocessing

Imports health data in CSV or JSON formats.

Normalizes timestamps and converts time zones if required.

Interpolates missing values and removes corrupted data segments.

Resamples data to consistent intervals (e.g., one minute or hourly).
This ensures that the dataset is consistent and ready for modeling.


Module 2: Feature Extraction and Modeling

Extracts statistical features using TSFresh such as mean, standard deviation, kurtosis, and others.

Applies Prophet for time-series trend modeling and forecasting.

Applies clustering algorithms such as KMeans and DBSCAN.

These techniques help in identifying patterns and deviations in the dataset.


Module 3: Anomaly Detection and Visualization

Anomalies are detected through the following methods:

Rule-based thresholds (e.g., heart rate spikes)

Forecast residual deviations

Outlier detection via clustering results

Detected anomalies are displayed on charts with annotations for clarity.


Module 4: Dashboard for Insights

Built using Streamlit for user interaction.

Allows users to upload files, run anomaly detection, and filter results.

Allows downloading reports in PDF or CSV formats.

This helps end-users interpret data easily through visual presentation.
