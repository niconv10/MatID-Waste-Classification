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

## 🌴 1. Problem & Motivation

### The Florida Context: Beauty & Boom
To understand the waste problem, we must look at the source. Florida is defined by two massive forces:

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="assets/maintenance_sample.png" width="400" alt="Florida Landscaping">
        <br>
        <b>The Standard of Beauty</b><br>
        <i>Millions of tons of Yard Waste from daily maintenance.</i>
      </td>
      <td align="center">
        <img src="assets/development_sample.png" width="400" alt="Construction Boom">
        <br>
        <b>The Construction Explosion</b><br>
        <i>Massive C&D debris from rapid urban development.</i>
      </td>
    </tr>
  </table>
</div>

> **The Result:** Landscape maintenance and rapid city development generate millions of tons of waste per year. **This is where the problem begins.**

---
### 🚛 From Source to Facility: The Convergence
Regardless of the source—whether it's a landscaping crew clearing a golf course or a demolition team clearing a lot—these materials share the same destination: **Material Recovery Facilities (MRFs).**

Hundreds of haulers transport this debris to MRFs daily. By the time these trucks arrive at the facility gate, the distinct sources often become a mixed, chaotic stream inside the dumpster.

### 🚜 The Industrial Challenge: The "Black Box" Truck
This creates a critical blind spot. The facility charges by material type (e.g., Concrete is cheaper to dump than Trash), but **they can't see inside the truck.**

Currently, they rely solely on the **driver's declaration**. When this declaration doesn't match reality (e.g., hiding organic waste inside a concrete load), the plant loses money.

#### The $2.1 Billion Financial Bleed
This lack of visual verification costs U.S. recycling plants an estimated **$2.1 Billion every year**.

```mermaid
pie title Annual Financial Losses in U.S. MRFs ($2.1B Total)
    "Fraud & Misclassification ($1.2B)" : 1200
    "Lack of Visual Proof ($630M)" : 630
    "Contaminated Loads ($210M)" : 210
