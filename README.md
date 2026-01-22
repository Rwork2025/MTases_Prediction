# ResiNet-GNN and SiteSpec-GNN: Leveraging Global and Local Structural Encodings for SAM-Binding Methyltransferase Classification

This repository provides data and code for **SAM-binding methyltransferase(MTases) classification** using two novel Graph Neural Network (GNN) models.  
The proposed framework integrates **global residue-level structural information** and **local site-specific patterns** to achieve accurate and interpretable predictions.

---

### 🔹 ResiNet-GNN
ResiNet-GNN captures **global structural characteristics** of proteins by modelling them as residue interaction graphs.  
This model is trained on the **PRN (Protein-wide Residue Neighbourhood) dataset**, where nodes represent amino acid residues and edges encode spatial interactions, enabling the learning of long-range dependencies relevant to various MTases.

### 🔹 SiteSpec-GNN
SiteSpec-GNN focuses on **local structural environments** surrounding functional SAM binding sites.  
It utilizes the **LRN (Ligand-centric Residue Neighbourhood) dataset**, which consists of one to all unique residue interaction set of active site, allowing the model to learn fine-grained local features critical for classification.

---

## Installation Instructions

The following setup was used to develop and run both ResiNet-GNN and SiteSpec-GNN models.

 pip install numpy pandas scikit-learn matplotlib seaborn tqdm
 
 pip install torch torchvision torchaudio
 
 pip install torch-geometric
 
 pip install torch-scatter torch-sparse torch-cluster torch-spline-conv

---

## How to load Datasets and run Model codes

### Loading the PRN Dataset
* Entering /ResiNet-GNN
* load `PRN_Dataset.pkl` as input file

### reproducing the result for ResiNet-GNN
* Entering /ResiNet-GNN
* run `Model.ipynb` to reproduce ResiNet-GNN result

### Loading the LRN Dataset
* Entering /SiteSpec-GNN
* load `LRN_Dataset.pkl` as input file

### reproducing the result for SiteSpec-GNN
* Entering /SiteSpec-GNN
* run `Model.ipynb` to reproduce SiteSpec-GNN result
  
---

## Contributors : 

### Lasya Durga Vadlamudi
Data Preprocessing and Model Development

### Lalitha Sreenidhi Sreekaram
Data Preprocessing and Model Development

### Kadam Mangal
Data Collection and Filtration

### Burra V L S Prasad 
Project Supervisor

