# Machine Learning Assisted Noise Classification and Mitigation in QKD

Code for my MS thesis. The work is described in the
preprint: https://arxiv.org/abs/2504.00718

## What this project does
- Simulates the BB84 and BBM92 quantum key distribution protocols on the
  IBM Qiskit simulator under two noise models: depolarizing and bit-flip.
- Builds QBER (quantum bit error rate) distributions for each noise type and
  uses them to select features.
- Applies PCA to reduce the number of features.
- Trains K-nearest neighbours, linear SVM and Gaussian naive Bayes classifiers
  to identify the noise type (98.8% to 100% accuracy for BB84 and BBM92).
- Implements BB84 over a quantum channel with the density matrix formalism to
  classify bit-flip and amplitude-damping noise (97% accuracy).
- Mitigates noise using singular value decomposition of the noisy matrices,
  followed by Bayesian optimization with scikit-learn.

## Repository structure
- [file or folder name]: [what it contains, e.g. BB84 simulation]
- [file or folder name]: [e.g. classifier training and evaluation]
- [file or folder name]: [e.g. SVD noise mitigation]

## How to run
1. Install the requirements: pip install qiskit scikit-learn numpy matplotlib
2. [Which file or notebook to run first]
3. [Which one reproduces the main results]

## Tools
Python, Qiskit, scikit-learn, NumPy, Matplotlib

## Citation
Banerjee S., Ashmi A., Panigrahi P. K. (2025). Machine Learning assisted
noise classification with Quantum Key Distribution protocols.
arXiv:2504.00718.
