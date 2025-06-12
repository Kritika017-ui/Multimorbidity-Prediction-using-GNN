Implement a Graph Convolutional Network (GCN) using the PyTorch Geometric library. The GNN aggregates neighborhood information from the disease graph to learn disease interdependencies. The trained Graph Neural Network (GNN) model effectively learned disease co-occurrence patterns from the MIMIC-III clinical dataset and was able to predict multimorbidity risk scores with high confidence. The model was tested using unseen ICD-9 code combinations. For each input, the system generated a risk score (a probability between 0 and 1) indicating the likelihood of a disease being comorbid with the input conditions.
Deployment:
Build an interactive Gradio-based web dashboard where users can:
Input ICD-9 codes manually or upload a CSV file.
Instantly receive comorbidity risk scores as output.     
Entire solution (training + deployment) is implemented and hosted on Google Colab, eliminating the need for a separate server or environment.






