# ai_project_synthetic_datasets
# Customer Churn Prediction using Neural Networks  
**Machine Learning Assignment – Neural Networks (Tasks 1–6)**  
**Author:** Sumathi  

---

## 📌 Project Overview  
This project builds a **binary classification model** to predict **customer churn** using a **feed‑forward neural network**.  
The notebook walks through all required tasks:

1. Dataset Understanding  
2. Data Preprocessing  
3. Neural Network Model Building  
4. Training & Evaluation  
5. Hyperparameter Experiments  
6. Final Reflection  

The project also includes a demonstration of **how neural networks learn internally** through:

- Forward pass  
- Loss calculation  
- Backpropagation  
- Parameter updates  

This satisfies the assignment requirement to explain the learning mechanics beyond simply training a model.

---

## 📂 Dataset  
The dataset contains customer attributes and a binary target variable:

- `churn = 1` → customer left  
- `churn = 0` → customer stayed  

The dataset is **highly imbalanced**, with very few churn cases.  
This required the use of **class weights** to ensure the model learns to detect churn.

---

## 🧹 Task 2 — Data Preprocessing  
Key preprocessing steps:

- Dropped non‑predictive ID column  
- Handled missing values  
- One‑hot encoded categorical features  
- Standardized numerical features  
- Performed train–test split with stratification  

---

## 🧠 Task 3 — Neural Network Model  
A neural network with:

- Input layer  
- Dense(32, ReLU)  
- Dense(16, ReLU)  
- Dense(1, Sigmoid)  

Compiled with:

- Loss: Binary Cross‑Entropy  
- Optimizer: Adam  
- Metric: Accuracy  

### 🔬 Learning Mechanics Demonstration  
A manual training step was implemented using `tf.GradientTape()` to show:

- Forward pass  
- Loss computation  
- Gradient calculation  
- Weight updates  

This demonstrates how neural networks learn internally.

---

## 🚀 Task 4 — Training & Evaluation  
Because the dataset is imbalanced, **class weights** were applied during training.

Evaluation metrics include:

- Accuracy  
- Precision, Recall, F1‑Score  
- Confusion Matrix  
- ROC‑AUC Score  

The model successfully improved **recall for the minority churn class**, which is the most important metric for churn prediction.

---

## 🔧 Task 5 — Hyperparameter Experiments  
Experiments were conducted by varying:

- Number of hidden units  
- Learning rate  

Each experiment was evaluated on the test set and summarized in a comparison table.

---

## 📝 Task 6 — Final Reflection  
The reflection discusses:

- Role of weights and biases  
- Importance of activation functions  
- Impact of learning rate  
- Underfitting vs. overfitting  
- Importance of handling class imbalance  

---

## 📊 Key Insights  
- High accuracy alone is misleading for imbalanced datasets  
- Class weights significantly improve minority‑class recall  
- Neural networks require careful tuning of architecture and learning rate  
- Manual gradient demonstration deepens understanding of model learning  

---

## 🛠 Technologies Used  
- Python 3.12  
- TensorFlow (CPU)  
- NumPy  
- Pandas  
- Scikit‑learn  
- Matplotlib  
- Seaborn  

---

## 📁 Repository Structure  
part-1-neural-network-analysis/
│
├── README.md
├── notebook.ipynb
├── requirements.txt
└── results/
    ├── model_comparison_table.png or .csv
    └── evaluation_outputs.png


---

## ✔ Conclusion  
This project demonstrates a complete neural‑network workflow for churn prediction, including theory, implementation, evaluation, and experimentation.  
It meets all assignment requirements and provides a clear explanation of how neural networks learn.


