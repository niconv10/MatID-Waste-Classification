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
Regardless of the source, these materials share the same destination: **Material Recovery Facilities (MRFs).** Thousands of haulers transport this debris to MRFs daily, creating a massive, mixed stream of incoming waste.

### 🏭 The MRF Workflow: A Typical Process
Understanding how these facilities operate is key to seeing the problem.

<div align="center">
  <img src="assets/mrf_sample.png" width="600" alt="Material Recovery Facility (MRF) Operation">
  <br>
  <i>A typical MRF operation where trucks dump mixed loads for processing.</i>
</div>

The standard process:

1.  **Truck Arrival & Weigh-in:** The truck arrives at the scale house, gets weighed, and the driver declares the material type to collect a ticket.
2.  **Dumping & Departure:** The truck proceeds to the tipping floor, dumps its material (into piles for either C&D or Yard Waste based on the declaration), and leaves.

> **The Critical Flaw:** At no point is there a reliable visual verification to ensure the dumped material matches the driver's declaration.

---
### 💸 The Consequence: A $2.1 Billion Annual Loss
Because facilities operate blindly based on manual input, they are essentially burning money. This lack of verification creates a massive financial bleed across the U.S. waste industry.

The industry loses an estimated **$2.1 Billion annually** due to three main factors:

1.  **Fraud & Misclassification ($1.2B):** This is not just driver deceit. It also happens inside the **Scale House**. Attendants or managers can manually modify material selections to declare cheaper rates (e.g., changing "Mixed Trash" to "Clean Concrete"), whether due to deliberate manipulation (collusion) or simple **human error**.
2.  **Lack of Visual Proof ($630M):** When clients dispute a bill, the facility has no photo evidence to prove what was actually dumped, forcing them to issue refunds.
3.  **Contaminated Loads ($210M):** Organic waste hiding in construction loads clogs shredders and ruins recyclable batches, driving up operating costs.

<div align="center">
  <img src="assets/financial_loss_chart.png" width="700" alt="$2.1 Billion Financial Loss Breakdown">
  <br>
  <i>Figure: Breakdown of losses driven by scale house manipulation, driver fraud, and lack of visual proof.</i>
</div>

> **The Solution:** MatID stops this bleeding by eliminating manual entry. We provide **automated classification** that cannot be manipulated by drivers or scale attendants.

---
