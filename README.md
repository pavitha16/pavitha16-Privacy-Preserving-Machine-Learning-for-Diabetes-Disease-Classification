# pavitha16-Privacy-Preserving-Machine-Learning-for-Diabetes-Disease-
##🔐 Privacy-Preserving Machine Learning for Diabetes Classification##
This project demonstrates the application of Differential Privacy (DP) techniques to machine learning models for diabetes classification using the Pima Indians Diabetes Dataset. It compares model performance and privacy guarantees across different privacy budgets (ε) using logistic regression with:

✅ Objective Perturbation

✅ Output Perturbation

✅ Non-Private Baseline

##📊 Dataset##
Pima Indians Diabetes Dataset

768 female patients (21+ years)

8 diagnostic features

Binary target: Outcome (0: Non-diabetic, 1: Diabetic)

📥 Download Dataset

🔍 Key Techniques
1. Objective Perturbation
Adds Gaussian noise to the loss function. Ensures (ε, δ)-DP.

2. Output Perturbation
Adds Laplace noise to model weights post-training. Ensures ε-DP.

3. Noise Mechanisms Used
Laplace

Gaussian

Exponential

Randomized Response

Shuffling

⚙️ Implementation Highlights
Feature Scaling with StandardScaler

Logistic Regression with/without Differential Privacy

Evaluation: Accuracy, AUC-ROC, Precision, Recall, F1

Privacy-Utility Tradeoff Analysis

📈 Lower ε = Higher privacy + Lower accuracy
📈 Higher ε = Lower privacy + Better accuracy

📌 Results
Objective Perturbation maintains better utility than Output Perturbation.

Epsilon values in the 1.0 – 5.0 range strike a practical balance between privacy and performance.

Visualization shows impact of noise at different privacy levels.

🧠 Conclusion
This implementation provides a practical framework to apply Differential Privacy in healthcare, balancing data confidentiality with model effectiveness.
