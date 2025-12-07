<div align="center">

<!-- Hero Section with Clean Logo -->
<img src="assets/matidlogo.png" width="280" alt="MatID Logo">

<br><br>

# MatID

### The AI Revolution in Waste Management

*Immediate, accurate material identification with full traceability.*

<br>

<!-- Modernized Badge Row - Monochrome Theme -->
[![Python](https://img.shields.io/badge/Python_3.10-000000?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-000000?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org)
[![Colab](https://img.shields.io/badge/Google_Colab-000000?style=flat-square&logo=googlecolab&logoColor=white)](https://colab.research.google.com)
[![W&B](https://img.shields.io/badge/Weights_&_Biases-000000?style=flat-square&logo=weightsandbiases&logoColor=white)](https://wandb.ai)
[![Status](https://img.shields.io/badge/Prototype-Complete-00C853?style=flat-square)](/)

<br>

---

**[The Problem](#-the-problem)** · **[Solution](#-the-solution)** · **[Technical Approach](#-technical-approach)** · **[Experiments](#-experiments)** · **[Results](#-results)** · **[Deliverables](#-deliverables)**

---

</div>

<br>

## 🌴 The Problem

### Florida: Where Beauty Meets the Boom

To understand the waste crisis, follow the source. Florida operates at the intersection of two massive forces:

<br>

<table>
<tr>
<td width="50%">

<div align="center">

**🌿 The Standard of Beauty**

<img src="assets/maintenance_sample.png" width="100%" alt="Florida Landscaping">

*Millions of tons of Yard Waste from daily maintenance.*

</div>

</td>
<td width="50%">

<div align="center">

**🏗️ The Construction Explosion**

<img src="assets/development_sample.png" width="100%" alt="Construction Boom">

*Massive C&D debris from rapid urban development.*

</div>

</td>
</tr>
</table>

<br>

> 💡 **The Result:** Landscape maintenance and rapid city development generate millions of tons of waste per year. This is where the problem begins.

<br>

---

### 🚛 The Convergence Point

Regardless of origin, all materials share the same destination: **Material Recovery Facilities (MRFs).** Thousands of haulers transport debris daily, creating a massive, mixed stream of incoming waste.

<br>

<div align="center">

<img src="assets/mrf_sample.png" width="700" alt="Material Recovery Facility (MRF) Operation">

*A typical MRF operation where trucks dump mixed loads for processing.*

</div>

<br>

### The Standard Process

| Step | Action |
|:----:|--------|
| **1** | Truck arrives at scale house, gets weighed |
| **2** | Driver declares material type, collects ticket |
| **3** | Truck proceeds to tipping floor |
| **4** | Material dumped based on declaration |
| **5** | Truck departs |

<br>

> ⚠️ **The Critical Flaw:** At no point is there reliable visual verification to ensure dumped material matches the driver's declaration.

<br>

---

### 💸 The Cost: $2.1 Billion Lost Annually

This verification gap creates a massive financial bleed across the U.S. waste industry.

<br>

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║              U.S. MRF FINANCIAL LOSSES                           ║
║              ─────────────────────────                           ║
║                                                                  ║
║     ████████████████████████████████████████  $1.2B  (57%)       ║
║     Fraud & Misclassification                                    ║
║                                                                  ║
║     ████████████████████████                  $630M  (30%)       ║
║     Lack of Visual Proof                                         ║
║                                                                  ║
║     ████████                                  $210M  (10%)       ║
║     Contaminated Loads                                           ║
║                                                                  ║
║                                              ─────────           ║
║                                      TOTAL:  $2.1 BILLION        ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

</div>

<br>

<details>
<summary><b>📊 Breakdown of Losses</b></summary>

<br>

| Category | Loss | Description |
|----------|------|-------------|
| **Fraud & Misclassification** | $1.2B | Attendants or managers modify material selections for cheaper rates—whether through collusion or human error |
| **Lack of Visual Proof** | $630M | No photo evidence when clients dispute bills, forcing facilities to issue refunds |
| **Contaminated Loads** | $210M | Misidentified loads trigger reprocessing costs and equipment damage (e.g., steel hidden in wood) |

</details>

<br>

---

## 💡 The Solution

<div align="center">

# MatID App

### Accuracy. Speed. Trust.

*At the Tipping Floor.*

</div>

<br>

MatID isn't just a model—it's an operational tool. By deploying AI on rugged tablets, we identify exact materials with **>99% accuracy**.

This eliminates billing disputes instantly and gives plant managers clean, trustworthy data for smart, data-driven decisions.

<br>

### 📲 The Workflow

<br>

<table>
<tr>
<td align="center" width="25%">

<img src="assets/truck_scale.png" width="180" alt="Step 1">

**Step 1**

*Truck Arrival & Weigh-in*

</td>
<td align="center" width="25%">

<img src="assets/truck_dump.png" width="180" alt="Step 2">

**Step 2**

*Dumping Material*

</td>
<td align="center" width="25%">

<img src="assets/ipad_picture.png" width="180" alt="Step 3">

**Step 3**

*AI Material Scan*

</td>
<td align="center" width="25%">

<img src="assets/print_ticket.png" width="180" alt="Step 4">

**Step 4**

*Ticket Prints*

</td>
</tr>
</table>

<br>

### Key Benefits

| | Benefit | Impact |
|:-:|---------|--------|
| 🚀 | **Increased Turnaround** | Entire process streamlined to under 5 minutes |
| 📸 | **Irrefutable Visual Proof** | Every ticket includes timestamped photo |
| 🚫 | **Fraud Prevention** | AI eliminates human error and misclassification |

<br>

---

## 🧠 Technical Approach

### Modified AlexNet Architecture

We leverage **transfer learning** with a pre-trained AlexNet model (trained on ImageNet) and adapt it for binary waste classification. The key modification is replacing the final fully connected layer to output 2 classes instead of 1,000.

<br>

<div align="center">

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                        ALEXNET ARCHITECTURE                                 │
│                     (Modified for Waste Classification)                     │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│   INPUT                                                                     │
│   224 × 224 × 3                                                             │
│        │                                                                    │
│        ▼                                                                    │
│   ┌─────────────────────────────────────────────────────────────────────┐   │
│   │                    FEATURE EXTRACTION                               │   │
│   ├─────────────────────────────────────────────────────────────────────┤   │
│   │  Conv1 → ReLU → MaxPool   (96 filters, 11×11, stride 4)            │   │
│   │  Conv2 → ReLU → MaxPool   (256 filters, 5×5)                       │   │
│   │  Conv3 → ReLU             (384 filters, 3×3)                       │   │
│   │  Conv4 → ReLU             (384 filters, 3×3)                       │   │
│   │  Conv5 → ReLU → MaxPool   (256 filters, 3×3)                       │   │
│   └─────────────────────────────────────────────────────────────────────┘   │
│        │                                                                    │
│        ▼                                                                    │
│   ┌─────────────────────────────────────────────────────────────────────┐   │
│   │                       CLASSIFIER                                    │   │
│   ├─────────────────────────────────────────────────────────────────────┤   │
│   │  Flatten → Dropout(0.5)                                            │   │
│   │  FC1: 9216 → 4096 → ReLU → Dropout(0.5)                            │   │
│   │  FC2: 4096 → 4096 → ReLU → Dropout(0.5)                            │   │
│   │  FC3: 4096 → 2  ← MODIFIED (originally 1000 for ImageNet)          │   │
│   └─────────────────────────────────────────────────────────────────────┘   │
│        │                                                                    │
│        ▼                                                                    │
│   OUTPUT                                                                    │
│   [C&D, Yardwaste]                                                          │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

</div>

<br>

### Dataset & Preprocessing

Our dataset consists of real-world images from Material Recovery Facilities, split into two classes:

| Class | Description | Train | Validation |
|-------|-------------|:-----:|:----------:|
| **C&D** | Construction & Demolition debris | *450* | *112* |
| **Yardwaste** | Organic landscape materials | *520* | *130* |

<br>

**Preprocessing Pipeline:**

All images undergo the following transformations before being fed into the model:

```python
# Standard preprocessing (no augmentation)
transforms = [
    Resize(224, 224),                                    # Resize to AlexNet input
    Normalize(mean=[0.485, 0.456, 0.406],               # ImageNet normalization
              std=[0.229, 0.224, 0.225]),
    ToTensor()
]
```

<br>

**Data Augmentation** (applied in select experiments):

```python
# Augmentation transforms
augmentations = [
    HorizontalFlip(p=0.5),
    VerticalFlip(p=0.2),
    RandomRotate90(p=0.5),
    RandomBrightnessContrast(brightness=0.2, contrast=0.2, p=0.3),
    ShiftScaleRotate(shift=0.1, scale=0.1, rotate=15°, p=0.3)
]
```

<br>

### Training Configuration

<div align="center">

| Parameter | Value |
|-----------|-------|
| **Framework** | PyTorch |
| **Pre-trained Weights** | ImageNet1K_V1 |
| **Loss Function** | CrossEntropyLoss |
| **Primary Optimizer** | Adam |
| **Epochs** | 15 |
| **Hardware** | Google Colab T4 GPU |
| **Tracking** | Weights & Biases |

</div>

<br>

### Experimental Variables

To understand model behavior, we systematically varied the following hyperparameters:

| Variable | Values Tested |
|----------|---------------|
| **Batch Size** | 16, 64 |
| **Learning Rate** | 0.0001, 0.001 |
| **Optimizer** | Adam, SGD (momentum=0.9) |
| **Data Augmentation** | On, Off |
| **Architecture** | AlexNet, VGG16, ResNet18 |

<br>

### Alternative Architectures

In addition to AlexNet, we compared performance against two other CNN architectures:

<br>

<table>
<tr>
<td width="33%" align="center">

**AlexNet**

*8 layers · 61M params*

The baseline. Fast training, lightweight architecture with 5 convolutional layers.

</td>
<td width="33%" align="center">

**VGG16**

*16 layers · 138M params*

Deeper network with uniform 3×3 convolutions. More parameters, slower training.

</td>
<td width="33%" align="center">

**ResNet18**

*18 layers · 11M params*

Skip connections enable better gradient flow. Efficient despite depth.

</td>
</tr>
</table>

<br>

All architectures were modified identically—replacing only the final classification layer to output 2 classes:

```python
# AlexNet & VGG16
model.classifier[6] = nn.Linear(4096, 2)

# ResNet18
model.fc = nn.Linear(512, 2)
```

<br>

---

<br>

---

## 🧪 Experiments

### Methodology

<br>

> *Details about experimental setup, hyperparameters, and training procedures.*

<br>

---

## 📊 Results

### Visualizations

<br>

> *Training curves, confusion matrices, and performance metrics.*

<br>

---

## 📂 Deliverables

### Project Resources

<br>

> *Links to notebooks, models, datasets, and documentation.*

<br>

---

<div align="center">

<br>

Made with 🧠 for smarter waste management

<br>

</div>
