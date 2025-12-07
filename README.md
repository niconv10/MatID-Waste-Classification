<div align="center">
  <img src="assets/matidlogo.png" width="300" alt="MatID Logo">
  
  <h1>The AI Revolution in Waste Management</h1>
  <h3>Immediate, accurate material identification with full traceability.</h3>

  <p>
    <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python" alt="Python">
    <img src="https://img.shields.io/badge/PyTorch-Deep_Learning-red?style=for-the-badge&logo=pytorch" alt="PyTorch">
    <img src="https://img.shields.io/badge/Google_Colab-T4_GPU-orange?style=for-the-badge&logo=googlecolab" alt="Google Colab">
    <img src="https://img.shields.io/badge/Weights_&_Biases-Tracking-gold?style=for-the-badge&logo=weightsandbiases" alt="WandB">
    <img src="https://img.shields.io/badge/Status-Prototype_Complete-success?style=for-the-badge" alt="Status">
  </p>
</div>

<br>

## 📑 Navigation
Use these links to jump to specific sections of the project:

1. [🔴 **The Problem & Motivation**](#-1-problem--motivation-the-florida-context)
2. [🧠 **Technical Approach (AlexNet)**](#-2-technical-approach-modified-alexnet)
3. [🧪 **Experiments & Methodology**](#-3-experimental-methodology)
4. [📊 **Results & Visualizations**](#-4-results--visualizations)
5. [📂 **Project Deliverables**](#-5-project-deliverables-resources)

---

## ♻️ 1. Problem & Motivation: The $2.1 Billion Visibility Gap
**The "Black Box" Truck Problem**

Every day, hundreds of trucks dump massive loads at Material Recovery Facilities (MRFs). The plant charges tipping fees based on material type, but they face a critical problem: **they can't see inside the truck.**

Currently, facilities rely solely on the **driver's declaration** of what they are carrying. This manual process is flawed and easily exploited. When the declaration doesn't match reality (e.g., stating "clean concrete" but dumping mixed trash), the plant loses significant money.

### The Financial Impact
This lack of verification costs U.S. recycling plants an estimated **$2.1 Billion every year**.

```mermaid
pie title Annual Financial Losses in U.S. MRFs ($2.1B Total)
    "Fraud & Misclassification ($1.2B)" : 1200
    "Lack of Visual Proof ($630M)" : 630
    "Contaminated Loads ($210M)" : 210

