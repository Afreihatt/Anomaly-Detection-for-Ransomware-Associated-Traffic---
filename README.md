# Anomaly-Detection-for-Ransomware-Associated-Traffic---

**README**: Ransomware Detection Using Anomaly Detection and Machine Learning
Overview
This research focuses on developing an advanced anomaly detection system to identify ransomware-associated network traffic using the UGRansome dataset. The study integrates traditional classification models with anomaly detection techniques to enhance ransomware detection capabilities. The research follows the Onion Model framework, employing a mixed-method approach, and evaluates various machine learning models and anomaly detection techniques to improve cybersecurity measures.

**Key Objectives:**
- Develop a Machine Learning Framework: Integrate deep learning and ensemble techniques for anomaly detection in real-time networks.
- Evaluate Anomaly Detection Techniques: Use methods like Isolation Forest, Local Outlier Factor (LOF), and One-Class SVM to detect ransomware-related anomalies.
- Compare Machine Learning Models: Assess the performance of models such as Decision Trees, Gradient Boosting, Random Forest, and Artificial Neural Networks (ANN) for ransomware detection.
- Enhance Cybersecurity Measures: Provide a structured approach to identifying and mitigating ransomware threats in network traffic.

**Dataset**
- The research uses the UGRansome dataset, which includes network traffic logs with features such as timestamps, protocols, IP addresses, ransomware families, and financial transactions (USD and BTC). The dataset is labeled, making it suitable for supervised anomaly detection.

**Dataset Features:**
Time: Timestamp of the event.

Protocol: Communication protocol used (e.g., TCP, UDP).

Flag: Network flow flags.

Family: Ransomware family (e.g., WannaCry, Locky).

BTC/USD: Bitcoin and USD values associated with transactions.

Netflow_Bytes: Volume of data transferred.

Prediction: Classification labels (Anomaly, Synthetic Signature, Signature).

**Methodology**
The research follows the Onion Model framework, which includes:

Philosophy: Positivism, focusing on measurable and data-driven methods.

Theory Development: Deductive approach, testing existing anomaly detection theories.

Methodological Choice: Mixed-method approach, combining quantitative and qualitative data.

Research Strategy: Longitudinal study to track anomalies over time.

Data Collection: Primary data from surveys with cybersecurity professionals and secondary data from the UGRansome dataset.

Data Analysis: Data cleaning, feature transformation, and exploratory data analysis (EDA) using tools like sweetviz.

Model Evaluation: Performance metrics include accuracy, precision, recall, and F1-score.

**Machine Learning Models**
The following models were evaluated for ransomware detection:

Decision Trees: Interpretable but prone to overfitting.

Gradient Boosting: High accuracy (98.3%) and balanced performance across all metrics.

Random Forest: Reduces overfitting and handles high-dimensional data.

Artificial Neural Networks (ANN): Excels at detecting complex patterns, achieving 97.9% accuracy.

Naive Bayes: Simple and fast but struggles with feature independence assumptions.

Anomaly Detection Techniques
Three unsupervised anomaly detection techniques were applied:

Isolation Forest: Detects anomalies by isolating data points, identifying 27,402 anomalies.

Local Outlier Factor (LOF): Detects anomalies based on local density, identifying 9,745 anomalies.

One-Class SVM: Detects anomalies by defining normal data boundaries, identifying 3,046 anomalies.

**Results**
- Gradient Boosting emerged as the best-performing model with 98.3% accuracy, followed by ANN with 97.9% accuracy.
- Isolation Forest detected the most anomalies, while One-Class SVM was the most conservative.

**Key insights from data visualizations:**

Dominant IP addresses (e.g., 1DA11mPS) and ransomware families (e.g., Locky, WannaCry) were identified.

Transaction patterns in USD and BTC were linked to ransom payments.

TCP protocol and specific flags (e.g., AF) were prevalent in ransomware traffic.

**Limitations**
- Data Incompleteness: Missing values in some columns.
- Static Dataset: Limited ability to detect new or evolving ransomware threats.
- Model Interpretability: Complex models like ANN and Gradient Boosting lack transparency.
- Survey Limitations: Small sample size and potential response bias.

**Recommendations**
Feature Selection: Perform feature selection to improve model efficiency.

Hyperparameter Optimization: Optimize hyperparameters for better model performance.

Explainable AI: Use techniques like SHAP or LIME to enhance model interpretability.

Real-Time Monitoring: Implement real-time data integration and model retraining to adapt to new threats.

Hybrid Approaches: Combine machine learning with rule-based systems for balanced anomaly detection.

**Future Work**
- Deep Learning Integration: Explore Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) for complex pattern recognition.
- Diverse Datasets: Incorporate more diverse network traffic data to improve generalizability.
- Hybrid Anomaly Detection: Combine multiple anomaly detection techniques for improved accuracy.
- Continuous Model Updates: Regularly update models with fresh data to adapt to evolving ransomware tactics.

**Conclusion**
This research demonstrates the effectiveness of machine learning and anomaly detection techniques in identifying ransomware-associated network traffic. Gradient Boosting and ANN are the top-performing models, while Isolation Forest is the most effective anomaly detection technique. Future work should focus on improving model interpretability, integrating real-time data, and exploring hybrid approaches for more robust ransomware detection.
