# Multimorbidity-Prediction-using-Graph Neural Network(GNNs)

This project presents an AI-based solution to predict multimorbidity risks in patients using Graph Neural Networks (GNNs) trained on clinical diagnosis data (ICD-9 codes) from the MIMIC-III dataset. It includes a web-based interface built with Gradio, allowing users to enter diagnosis codes and receive comorbidity risk scores in real-time.

---

##  Features

- Predicts comorbid disease risks from ICD-9 diagnosis codes
- Built using Graph Convolutional Networks (GCNs) in PyTorch Geometric
- Interactive dashboard built with Gradio
- Trained on real-world clinical data from MIMIC-III
- Accepts both manual input and CSV file uploads

---


## 📚 Dataset

- **MIMIC-III Clinical Database Demo (1.4)**  
  Source: Kaggle  
  🔗 https://www.kaggle.com/datasets/montassarba/mimic-iii-clinical-database-demo-1-4

---

## 🧰 Technologies Used

| Tool/Library       | Purpose                                    |
|--------------------|--------------------------------------------|
| Python 3.x         | Core programming language                  |
| PyTorch            | Deep learning framework                    |
| PyTorch Geometric  | GNN model development                      |
| Gradio             | Building the interactive web dashboard     |
| Pandas, NumPy      | Data handling and processing               |
| NetworkX           | Graph construction and analysis            |
| Scikit-learn       | Evaluation metrics (accuracy, ROC-AUC)     |

---

## 🧠 Model Overview

- Diseases (ICD-9 codes) are represented as **nodes** in a graph.
- Edges between nodes represent **co-occurrence** in patient records.
- A **Graph Convolutional Network (GCN)** learns disease relationships and predicts **risk scores** for possible comorbid conditions.
- Output: A risk score (0 to 1) indicating the likelihood of each comorbidity.

---

## 🚀 How to Use

### ▶️ Run on Google Colab:

Click below to open the full notebook:  
👉 [Open Colab Notebook](https://colab.research.google.com/drive/1Arvy234OSzjdw-l036CgXAKbeJJ9up9w?usp=sharing)

### 📌 Steps:

1. Run all cells in order (data processing → training → dashboard).
2. Enter ICD-9 codes manually in the dashboard, or upload a CSV file.
3. View predicted **risk scores** in the dashboard output.

---

## 📊 Example Output

**Input ICD-9 Codes**: `40391, 42731`

| ICD-9 Code | Risk Score |
|------------|------------|
| 40391      | 0.99       |
| 42731      | 0.81       |

> The model outputs the likelihood of each condition being comorbid based on learned disease relationships.

---

## 🔮 Future Improvements

- Support for **ICD-10** codes for broader applicability.
- Incorporation of **patient demographics** (e.g., age, gender).
- Use of **Graph Attention Networks (GATs)** for better explainability.
- Integration with **real-time hospital EHR systems**.

---

## 📖 References

- **MIMIC-III Dataset**  
  https://www.kaggle.com/datasets/montassarba/mimic-iii-clinical-database-demo-1-4
- **Graph Convolutional Networks Paper**  
  Kipf & Welling (2016) – https://arxiv.org/abs/1609.02907
- **PyTorch Geometric**  
  https://pytorch-geometric.readthedocs.io/
- **Gradio**  
  https://www.gradio.app/

---

## 👨‍💻 Author

**Kritika Rana**  
📧 Email: [kritikar42@gmail.com]  
🏫 Institution: [Chandigarh University, BE-CSE(AIML)]

---

⭐ If you found this project helpful, feel free to star the repo and share it!



