# Quantum Image Classification with QSVM & QCNN

## Project Overview
This repository explores quantum machine learning techniques for image classification, comparing quantum models (QSVM, QCNN) with classical counterparts (SVM, CNN). Key innovations include:  
- **INEQR**: Quantum image representation for efficient statevector encoding.  
- **QHED**: Quantum Hadamard Edge Detection for data compression.  
Tested on MNIST, CIFAR-10, and custom datasets with resized/grayscale images.

## Key Findings
- **QSVM** achieved **100% training accuracy** but suffered from overfitting (50% testing accuracy).  
- **INEQR-enhanced QSVM** balanced performance (93% train, 60% test accuracy).  
- **QCNN** underperformed classical CNN (**18.1% accuracy**) due to hardware constraints (image downsizing, qubit limits).  
- Quantum methods showed **longer computation times** (e.g., QSVM training took 22s vs. SVM’s 0.02s).  

## Repository Contents
- `Final_Project_Report.pdf`: Full technical report with methodology, results, and discussions.  
- Main Code notebooks:  
  - `INEQR_QSVM.ipynb`: Quantum SVM with INEQR image encoding.  
  - `QHED3.ipynb`: Quantum CNN with edge detection preprocessing.  
  - Classical baseline implementations (SVM, CNN).  

## Dependencies
- Python 3.8+  
- Libraries: `qiskit`, `pennylane`, `tensorflow`, `scikit-learn`, `piQture` (for INEQR).  
- Quantum backends: IBM Quantum Experience, local simulators.  

## Citation
If referencing this work, please cite:  
> Avi Veeramoothoo & Munia Humaira. *Novel Quantum Image Representation & Data Compression for Classifying Images via Quantum Classifiers & Neural Networks*. University of Waterloo, 2024.  

**Note**: Datasets used:  
- [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)  
- [MNIST](http://yann.lecun.com/exdb/mnist/)  

## Contributors
- **Munia Humaira**: QSVM, INEQR implementation.  
- **Avi Veeramoothoo**: QCNN, QHED integration.  

For questions, contact [Munia](mailto:munia.humaira@uwaterloo.ca).  