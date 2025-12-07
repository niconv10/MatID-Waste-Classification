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

## 🌴 1. Problem & Motivation: The Florida Context
**"Beauty vs. The Boom"**

In Florida, we live in a dichotomy. We see perfectly manicured golf courses and neighborhoods daily (generating massive **Yard Waste**), and simultaneously, we see a skyline filled with construction cranes (generating **C&D Debris**).

These two massive streams often end up mixed in the same dump trucks. Currently, waste facilities struggle to distinguish them efficiently at the entry gate. This leads to critical operational failures:

* **💸 Revenue Loss:** Facilities charge incorrect tipping fees because they can't accurately estimate the ratio of materials.
* **⚠️ Contamination:** Organic waste hides inside recyclable concrete loads, ruining the recycling batch.
* **📉 Lack of Traceability:** There is no visual proof for clients to justify billing adjustments.

**MatID** solves this by using Computer Vision (AlexNet) to automatically classify waste truck loads at the gate, providing **visual proof and automated billing**.

### 📸 The Dataset: Real-World Complexity
To train our model, we collected a dataset of real-world images from local facilities. The challenge lies in the visual similarity between "dirty wood" (C&D) and "branches" (Yard Waste).

| Class A: Construction (C&D) | Class B: Yard Waste |
| :---: | :---: |
| <img src="assets/cnd_sample.png" width="400" alt="Construction Waste"> | <img src="assets/yard_sample.jpeg" width="400" alt="Yard Waste"> |
| *Concrete, bricks, rebar, and lumber.* | *Vegetation, branches, grass, and stumps.* |

---
