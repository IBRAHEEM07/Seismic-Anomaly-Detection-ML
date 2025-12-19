
# Anomaly Detection in Seismic Data using Threshold-Based Machine Learning


## 📌 Overview

This project focuses on **detecting frequency anomalies in seismic data** introduced during the frequency compensation process. Such anomalies can negatively impact seismic interpretation in **oil and gas exploration**.

The proposed solution combines a **threshold-based anomaly detection approach** with a **Decision Tree supervised machine learning model**, achieving high accuracy and robustness on real seismic datasets.

---

## 🎯 Objectives

* Detect frequency artifacts in seismic data
* Improve seismic data reliability for geological interpretation
* Compare machine learning–based anomaly detection with traditional methods
* Handle class imbalance using **SMOTE**

---

## 🧠 Methodology

1. **Dataset**

   * Facies Classification Benchmark (Netherlands F3 Block)
   * SEGY format
   * Selected 20 in-line slices (each: 255 × 601)

2. **Preprocessing**

   * Conversion from 3D to 2D seismic slices
   * Threshold-based labeling (normal vs anomaly)
   * SMOTE applied to balance classes

3. **Model**

   * Decision Tree Classifier
   * Train/Test split: 80/20
   * Supervised learning

4. **Evaluation Metrics**

   * Accuracy
   * Precision
   * Recall
   * Specificity
   * F1-Score (primary metric for anomaly detection)

---

## 📊 Results

| Metric    | Testing Performance |
| --------- | ------------------- |
| Accuracy  | 94%                 |
| Precision | 93%                 |
| Recall    | 95%                 |
| F1-Score  | 94%                 |

* Successfully detects **subtle frequency anomalies**
* Outperforms traditional threshold-only approaches
* Effective on large-scale seismic datasets

---

## 📈 Visual Outputs

* Frequency spectrum analysis
* Amplitude distribution
* Anomaly distribution across traces and time samples
* Confusion matrices (training & testing)
* Detected anomaly maps on seismic slices

---

## 🛠️ Tech Stack

* **Python 3**
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* segyio
* Google Colab

---

## 📁 Project Structure

```
├── data/
│   └── seismic_data.segy
├── notebooks/
│   └── anomaly_detection.ipynb
├── src/
│   ├── preprocessing.py
│   ├── thresholding.py
│   ├── model.py
│   └── evaluation.py
├── results/
│   └── figures/
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/seismic-anomaly-detection.git

# Install dependencies
pip install -r requirements.txt

# Run the notebook or scripts
```

---

## 🔮 Future Work

* Type-based anomaly classification
* Integration of domain-specific seismic features
* Adaptive noise filtering in frequency domain
* Scaling to larger 3D seismic datasets
* Testing deep learning models for comparison

---

## 📚 References

* Wang et al., *IEEE TGRS*, 2024
* Alaudah et al., *Facies Classification Benchmark*, 2019
* Rahma Putra et al., *Earth Science Informatics*, 2024

---

## 👤 Author

**Muhammad Talha Khan, Muhammad Ibraheem, Syed Maisum Abbas**
*Machine Learning | Seismic Data Analysis | Oil & Gas Applications*

