# ERGCNPPIS: Enhanced Residual Graph Convolutional Network for Protein-Protein Interaction Site Prediction

Accurate prediction of protein interaction sites is essential for understanding many biological processes. The Residual Graph Convolutional Network for Protein-Protein Interaction Site Prediction (RGCNPPIS) model has been successful by leveraging sequence features and spatial neighborhood information. However, its performance can be further improved in accuracy and efficiency.

RGCNPPIS captures local and global structural, evolutionary, and sequence-based features but overlooks critical physicochemical properties important for protein interactions and suffers from feature redundancy. To address these limitations, we propose **Enhanced RGCNPPIS (ERGCNPPIS)**. This enhanced model incorporates three key physicochemical features—**electrostatic potential**, **hydrogen-bonding propensity**, and **solvent-accessible surface area**—to provide better feature representation of protein structures and improve the understanding of protein interactions.

In addition to these enhancements, we perform **feature ablation analysis** to systematically evaluate and identify the most important features for the model. ERGCNPPIS has been evaluated on the **Test_71** and **Test_315** benchmark datasets, achieving a binary accuracy of **90.2%** on Test_71 and **93.7%** on Test_315. The model also shows significant improvements in key metrics, including a **31.9% increase in F1 score** and **42.8% improvement in the Area Under Precision-Recall Curve** on Test_315.

## System Requirements

To run ERGCNPPIS, you need the following dependencies:

- **Python** 3.10.13
- **NumPy** 1.26.4
- **Pandas** 1.1.0
- **PyTorch** 1.12.1 (GPU required)
- **Scikit-learn** 1.4.2

## Dataset

Before running the code, please follow these steps:

1. Unzip the compressed files located in the `Feature` folder.
2. Place the files `distance_map(part1).rar`, `distance_map(part2).rar`, and `distance_map(part3).rar` into a folder named `distance_map`.

## Usage

To train or evaluate the model, use the following commands:

- **Training the Model:**
  ```bash
  python train.py
  ```

- **Evaluating the Model:**
  ```bash
  python test.py
  ```

## Citation

If you find this work useful in your research, please cite our paper:

```

```

---
