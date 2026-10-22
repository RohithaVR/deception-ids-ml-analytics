# Deception-Based Intrusion Detection & ML Log Analysis

## Project Overview
This repository contains a full-cycle engineering framework for deploying deception infrastructure and utilizing machine learning algorithms to isolate malicious cyber operations. By deploying low- and high-interaction honeypots, traffic signatures were ingested into a data pipeline, optimized via feature engineering, and classified using anomaly detection algorithms.

---

## Technical Architecture & Pipeline
1. **Deception Deployment:** Configured tactical low-interaction and high-interaction honeypots utilizing **Dionaea, Kippo, and Modern Honey Network (MHN)** to capture reconnaissance maps and brute-force indicators.
2. **SIEM Ingestion:** Built optimized **Splunk dashboards** to monitor continuous network interactions, aggregate telemetry, and isolate live authentication attacks.
3. **Data Science Sandbox:** Formatted, parsed, and cleaned an evaluation dataset containing over **35,000 security logs** to map precise traffic behaviors.
4. **Machine Learning Classifier:** Engineered an optimized **Random Forest Anomaly Classifier**, achieving a **95% classification accuracy rating** distinguishing benign traffic patterns from actively malicious attacks.
5. **Defensive Validation:** Simulating adversarial campaigns within a sandbox utilizing **Nmap** and **Metasploit** to baseline detection alerts.

---

## Repository Structure & Components

* **`Synthetic_Honeypot_Logs_Analysis.ipynb`**
  Exploratory Data Analysis (EDA) notebook. Parses raw unstructured honeypot log directories, manages missing values, and visualizes geographic/port threat distributions.
* **`DATA_SIMULATION.ipynb`**
  Ingestion logic script modeling production honeypot telemetry profiles to consistently evaluate pipeline stress testing.
* **`Honeypot_Logs_ML_Model.ipynb`**
  Core model deployment file. Implements supervised classification frameworks, runs hyperparameter tuning for the **Random Forest Classifier**, and maps out performance metrics (Confusion Matrix, Precision-Recall curves).

---

## Tooling & Frameworks
* **Deception/SecOps:** Splunk Enterprise, Modern Honey Network (MHN), Dionaea, Kippo, Kali Linux, Nmap, Metasploit
* **Data Science Pipeline:** Python, Jupyter Notebooks, Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

---

## Metric Highlights
* **Log Footprint Analysed:** 35,000+ individual security log events.
* **Classifier Target Accuracy:** **95.2%** via optimized ensemble validation structures.
