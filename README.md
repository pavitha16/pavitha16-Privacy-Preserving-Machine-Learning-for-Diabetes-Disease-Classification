# 🔐 Privacy-Preserving Machine Learning for Diabetes Disease Classification

This project explores the application of **Differential Privacy (DP)** to machine learning models for **diabetes classification** using the **Pima Indians Diabetes Dataset**. It evaluates the **privacy-utility trade-off** across various privacy budgets (ε) using **Logistic Regression** with:

- ✅ Objective Perturbation  
- ✅ Output Perturbation  
- ✅ Non-Private Baseline  

---

## 📊 Dataset

- **Name**: Pima Indians Diabetes Dataset  
- **Instances**: 768 female patients (21+ years old)  
- **Features**: 8 diagnostic attributes  
- **Target**: `Outcome` (0 = Non-diabetic, 1 = Diabetic)

🔗 [Download Dataset](https://drive.google.com/file/d/14aqc4rK8hcFSES-SlRztGBlGca-QuIDd/view?usp=sharing)

---

## 🔍 Key Techniques

### 1. Objective Perturbation
- Adds **Gaussian noise** to the loss function.
- Ensures **(ε, δ)-Differential Privacy**.
- Optimized using **L-BFGS-B**.

### 2. Output Perturbation
- Adds **Laplace noise** to trained model weights.
- Ensures **ε-Differential Privacy**.
- Simpler, but less utility at strict privacy levels.

### 3. Noise Mechanisms Used
- **Laplace Mechanism**  
- **Gaussian Mechanism**  
- **Exponential Mechanism**  
- **Randomized Response**  
- **Shuffling Mechanism**

---

## ⚙️ Implementation Highlights

- 🔧 Feature scaling using `StandardScaler`
- 🔄 Train-test split (80/20) with stratified sampling
- 📈 Evaluation Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - AUC-ROC
- 📉 Privacy-Utility Tradeoff Analysis
- 📊 Visualization of noise impact on data distribution

---

## 📈 Privacy-Utility Insights

- **Lower ε → Higher Privacy → Lower Accuracy**
- **Higher ε → Lower Privacy → Higher Accuracy**

### 🔎 Results Summary:
- Objective Perturbation outperforms Output Perturbation, especially at low ε.
- Epsilon in **1.0 – 5.0** provides a practical balance of privacy and utility.
- Visualization shows progressive data distortion as ε decreases.

---

## 🧠 Conclusion

This implementation demonstrates how **Differential Privacy** can be effectively applied to **healthcare datasets**, preserving **patient confidentiality** while maintaining strong **predictive performance**. It offers a practical framework for privacy-aware machine learning in sensitive domains.

---

## 📁 Code & Data

- 📂 [Code Repository](https://drive.google.com/file/d/1uV9FGOaUDWaq31RHoEL_Vu2NB6hf5Wm_/view?usp=sharing)
- 📄 [Dataset Link](https://drive.google.com/file/d/14aqc4rK8hcFSES-SlRztGBlGca-QuIDd/view?usp=sharing)

---

