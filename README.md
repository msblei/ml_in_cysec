# Machine Learning in Cybersecurity

Interactive notebooks for learning how to apply machine learning to cybersecurity problems. Runs entirely in the browser via [JupyterLite](https://jupyterlite.readthedocs.io/).

## Notebooks

### BFH 1 — Android Malware Detection

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/msblei/ml_in_cysec/blob/main/content/BFH_1_Android_Malware_Detection.ipynb)

Classify Android apps as malware or benign using the [Drebin dataset](https://www.mlsec.org/docs/2014-ndss.pdf) (binary features for permissions, API calls, and class usage).

- **Session 1 — Logistic Regression:** Baseline binary classifier with ROC curve analysis
- **Session 2 — Support Vector Machine:** Configurable kernel (linear, poly, rbf, sigmoid), regularization strength, and decision boundary visualization via PCA

### BFH 2 — DDoS Detection with Neural Networks

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/msblei/ml_in_cysec/blob/main/content/BFH_2_Neural_Network.ipynb)

Detect DDoS attacks in cloud network traffic using a neural network trained on the [BCCC Cloud Packet DDoS 2024 dataset](https://www.mdpi.com/2078-2489/15/4/195) (319 network flow features).

- Uses scikit-learn's `MLPClassifier`
- Students tune: hidden layer sizes, activation function, learning rate, regularization, batch size, and early stopping
- Outputs training loss curve and detailed evaluation metrics (accuracy, precision, recall, F1, F-beta, TPR, FPR, confusion matrix)

## Run in the browser

This project is deployed as a JupyterLite site on GitHub Pages:

**https://msblei.github.io/ml_in_cysec**

Requirements: Firefox 90+ or Chromium 89+

## References

- Arp, D. et al. _"Drebin: Effective and explainable detection of android malware in your pocket."_ NDSS 2014.
- Shafi, M. et al. _"Toward generating a new cloud-based Distributed Denial of Service (DDoS) dataset and cloud intrusion traffic characterization."_ Information 15.4 (2024): 195.
