# Bayesian Classification with Gaussian Processes (Reproduction Study)

This repository presents a reproduction and extension of the paper:

**Williams and Barber (1998)** – *Bayesian Classification with Gaussian Processes*.

We revisit this foundational work through theoretical reimplementation and practical experimentation using two real-world datasets: **Crabs** and **Pima Indians Diabetes**.

---

## Objectives

- Understand and implement Gaussian Process classification using the Laplace approximation.
- Evaluate GP models on different datasets and preprocessing pipelines.
- Compare GPs to classical classifiers like SVM.
- Explore library limitations (GPy, GPflow) and practical implementation barriers.

---

## Crabs Dataset

- Biometric data for 200 crabs from two species (Blue, Orange) and two sexes.
- Binary classification performed using selected numerical features.
- Investigated the impact of feature scaling and kernel sensitivity.

---

## Pima Indians Diabetes Dataset

- Dataset includes 768 samples with 8 medical predictor variables.
- Binary outcome: diabetic (1) or not (0).
- Used for additional experimentation with kernels (RBF, Matern) and preprocessing effects.

---

## Key Takeaways

- Laplace approximation is challenging to implement manually but instructive.
- GP models are highly sensitive to feature scaling.
- StandardScaler and MinMaxScaler both yield different hyperparameter behaviors.
- GPy proved easier to use than GPflow due to TensorFlow compatibility issues.
- SVM outperformed GP in accuracy and training time on both datasets, but lacked uncertainty estimation.

---

##  Notes

- GPflow notebooks may fail if TensorFlow version is not compatible.
- Manual Newton optimization steps were coded to better understand posterior approximation.

---

## Reference

> Williams, C. K. I., & Barber, D. (1998). Bayesian classification with Gaussian processes. *IEEE Transactions on Pattern Analysis and Machine Intelligence*, 20(12), 1342–1351.

---

For any questions or contributions, feel free to open an issue or fork the repository.
