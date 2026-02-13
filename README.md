# 🔥 MNIST Representation & Spatial Awareness Study  
**Repo:** mnist-fcnn-representation-study

## 📌 Overview
This project studies how Fully Connected Neural Networks (FCNNs) learn image representations and whether they understand spatial structure.

Two experiments were conducted on MNIST:
1. Weight visualization of first hidden layer neurons  
2. Training on pixel-scrambled MNIST  

---

## 🧪 Experiment 1 — Weight Visualization
- Trained FCNN on MNIST  
- Extracted first-layer neuron weights  
- Reshaped to 28×28 and visualized as heatmaps  

**Observation:**  
Neurons capture global stroke/intensity patterns but lack localized spatial awareness.

---

## 🧪 Experiment 2 — Scrambled MNIST
- Applied fixed random pixel permutation to all images  
- Trained same FCNN architecture  

**Result:**  
Accuracy remained nearly identical to normal MNIST.

**Insight:**  
FCNN treats images as flat vectors and lacks spatial inductive bias.

---

## 🛠 Tech Stack
- PyTorch / TensorFlow  
- NumPy  
- Matplotlib  

---

## 🎯 Core Takeaway
High accuracy does not imply spatial understanding.  
FCNNs perform well on MNIST without learning true 2D structure — explaining why CNNs dominate vision tasks.
