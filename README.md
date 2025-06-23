# ⚡ Smart Grid Fault Detection and Self-Healing System

This project is an AI-enabled solution for real-time fault detection and self-healing in smart electrical grids. It uses a Random Forest machine learning model to classify fault types based on input grid parameters and recommends recovery actions automatically.

## 🧠 Problem Statement

Power grids often suffer from various faults such as phase failures, transformer issues, or main supply interruptions. Manual fault handling leads to longer downtimes and potential hazards. This system provides an intelligent way to detect faults and guide corrective actions in real time.

---

## 🚀 Features

- Train a machine learning model to classify grid faults
- Predict fault types from real-time parameters
- Recommend automatic self-healing actions
- Visualize grid stability and recovery
- Simulate live parameter behavior using Streamlit
- Maintain a log of all detected faults and actions

---

## 📊 Dataset

The dataset smart_grid_fault_data.csv includes:

- voltage – Line voltage in volts  
- current – Line current in amperes  
- frequency – Power frequency in Hz  
- power_factor – Load power factor  
- fault_type – Encoded fault category (0-4)

---

## 🔧 Methodology

1. *Data Preprocessing*
   - Categorical encoding for fault_type
   - Train-test split (80/20)

2. *Model Training*
   - RandomForestClassifier from scikit-learn
   - Accuracy and classification metrics

3. *Self-Healing Logic*
   - Fault types mapped to recovery actions (rerouting, UPS switch, etc.)
   - Simulated voltage-time graphs for each action

4. *Web Dashboard*
   - Built using Streamlit
   - Live parameter sliders
   - Fault detection button
   - Dynamic graph-based simulation

---

## 📁 Project Structure
├── app.py                       # Streamlit dashboard ├── fault_detection_model.pkl   # Trained ML model ├── smart_grid_fault_data.csv   # Dataset ├── fault_logs.txt              # Log file for detections ├── requirements.txt            # Project dependencies └── README.md                   # Project documentation
---

## ▶️ Run the Project

1. Install requirements:
   ```bash
   pip install -r requirements.txt
