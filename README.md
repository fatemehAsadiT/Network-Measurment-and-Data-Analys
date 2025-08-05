# Network Measurement and Data Analysis Lab

This repository contains all lab assignments from the *Network Measurement and Data Analysis Lab* course at Politecnico di Milano.  
The course consists of two main parts: **Network Measurement Lab** and **Network Data Analysis Lab**.  
The first part focuses on collecting network data through active and passive measurement techniques, traffic classification, and Wi-Fi sniffing.  
The second part focuses on analyzing network data using machine learning techniques.

---

## Part 1 – Network Measurement Lab
This part of the course focuses on methods for collecting and analyzing network data through both active and passive measurements, traffic classification, and Wi-Fi sniffing techniques. It includes three individual assignments.

### Homework 1 – Active Measurements
- **Objective:** Measure the relationship between Round-Trip Time (RTT) and the physical distance between network endpoints.
- **Key Steps:**
  - Use tools like `ping` to collect RTT data from multiple servers worldwide.
  - Compute geographical distances using latitude/longitude coordinates.
  - Plot RTT vs. distance and fit a linear model to estimate RTT per km.
- **Skills Applied:** Python scripting, ICMP measurements, `geopy` distance calculations, data visualization, regression analysis.

### Homework 2 – Website Fingerprinting
- **Objective:** Identify visited websites by analyzing only encrypted HTTPS traffic.
- **Key Steps:**
  - Capture `.pcap` traffic for visits to specific news websites.
  - Extract bi-directional flow features (packet counts, bytes, sizes, inter-arrival times).
  - Train a k-NN classifier and evaluate accuracy on test data, including temporal variations.
  - Implement an additional feature-based approach using cumulative packet size traces.
- **Skills Applied:** Network packet capture (`tcpdump`, `tshark`), feature extraction, machine learning classification, accuracy evaluation, confusion matrix analysis.

### Homework 3 – MAC Address De-randomization
- **Objective:** Implement an online clustering technique to group randomized MAC addresses belonging to the same physical device.
- **Key Steps:**
  - Analyze Wi-Fi probe request features to identify locally administered MAC addresses.
  - Group probe requests into clusters based on feature similarity.
  - Tune parameters to maximize clustering performance (v-measure, completeness, homogeneity).
  - Validate the method on labeled and challenge datasets.
- **Skills Applied:** Wi-Fi sniffing, MAC address analysis, clustering algorithms, performance evaluation, privacy and security considerations.

---

## Part 2 – Network Data Analysis Lab
This part focuses on applying data analysis and machine learning techniques to real-world networking problems, including application traffic classification, optical network quality estimation, and traffic prediction.

### Homework 1 – Application Flow Identification
- **Objective:** Identify traffic flows of different applications (e.g., YouTube, OneDrive) using machine learning classifiers such as Logistic Regression and XGBoost.
- **Key Steps:**
  - Dataset creation and preprocessing
  - Feature distribution visualization
  - Hyperparameter tuning with cross-validation
  - Model training and performance evaluation
  - Multi-class application identification
- **Skills Applied:** Python, scikit-learn, data preprocessing, ML model evaluation, PCA visualization.

### Homework 2 – Quality of Transmission (QoT) Estimation in Optical Networks
- **Objective:** Predict the QoT (SNR) for lightpaths in optical networks to optimize modulation format selection and reduce resource waste.
- **Key Steps:**
  - Raw data exploration and feature extraction
  - Visualization of correlations between features and SNR
  - Training Neural Networks and Linear Regression models
  - Evaluating impact of using single vs multiple features
  - Analysis of inaccurate predictions and safety margins
  - Studying effects of uncertain fiber span lengths
- **Skills Applied:** Python, regression models, neural networks, performance metrics (MSE, R²), feature impact analysis.

### Homework 3 – Traffic Prediction
- **Objective:** Predict mobile network traffic using Artificial Neural Networks (ANN) and Long Short-Term Memory (LSTM) networks.
- **Key Steps:**
  - Preprocessing of Telecom Italia Milano GRID dataset (CDRs)
  - Feature extraction and dataset preparation for ANN and LSTM
  - Model training, evaluation, and comparison (ANN vs LSTM)
  - Assessment of over/under-provisioning costs for resource allocation
- **Skills Applied:** Python, Keras/TensorFlow, time series prediction, ANN, LSTM, performance metrics (MSE, MAE, R²).

---

## Author
**Fatemeh Asadi Tirtashi**  
Politecnico di Milano – Telecommunications Engineering
