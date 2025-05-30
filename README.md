# 🧠 PCA  on Handwritten Digits Dataset.

This project demonstrates the application of **Principal Component Analysis (PCA)** and **Logistic Regression** on the **`load_digits()`** dataset from `scikit-learn`. It includes:

- Training a **Logistic Regression classifier** on the **original 64-dimensional** data
- Applying **PCA for dimensionality reduction**
- Retraining Logistic Regression on the **PCA-reduced data**
- Comparing **model accuracy**, **performance**, and **execution time** before and after PCA

---

## 📌 Table of Contents

- [About the Dataset](#about-the-dataset)
- [Project Goals](#project-goals)
- [Technologies Used](#technologies-used)
- [Results](#results)
- [Key Takeaways](#key-takeaways)

---

## 📊 About the Dataset

The `load_digits()` dataset contains:

- **1797** grayscale images of handwritten digits (**0 to 9**)
- Each image is **8×8 pixels**, flattened into a **64-dimensional vector**
- Pixel values range from **0 (white)** to **16 (black)**
- Each entry has a corresponding **label (0–9)**

---

## 🎯 Project Goals

- Train a **Logistic Regression classifier** on original high-dimensional data
- Use **PCA** to reduce dimensionality while preserving variance
- Compare **classification accuracy and efficiency** before and after PCA

---

## 🧰 Technologies Used

- Python 3.x
- `scikit-learn` – for loading data, PCA, and Logistic Regression
- `matplotlib` & `seaborn` – for data visualization
- `numpy`, `pandas` – for data processing

---

## ✅ Results

| Metric                     | Without PCA (64 features) | With PCA (29 components) |
|----------------------------|---------------------------|---------------------------|
| Accuracy                   | **97.22%**                | **96.44%**                |
| Number of Features         | 64                        | 29                        |
| Dimensionality Reduction   | ❌                        | ✅ ~55% fewer features     |
| Training Time              | Slightly higher           | Slightly faster           |

---

## ✨ Key Takeaways

- Logistic Regression achieves **97.22% accuracy** on the original 64-feature space.
- After reducing the features to **29 principal components** using PCA, the model still maintains a strong **96.44% accuracy**.
- PCA helped in **reducing dimensionality by ~55%**, while **retaining over 96% classification performance**.
- This trade-off is often valuable when working with larger, high-dimensional datasets where training speed and generalization matter.

---

## 🤝 Contributions
Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

