# DIDO

PyTorch implementation for Discretization-Induced Dirichlet Posterior for Robust Uncertainty Quantification on Regression (AAAI 2024).  
[Paper](https://arxiv.org/abs/2308.09065)

## Abstract

Uncertainty quantification is critical for deploying deep neural networks (DNNs) in real-world applications. In this work, we advance an Auxiliary Uncertainty Estimator (AuxUE), which is one of the most effective means to estimate the uncertainty of the main task prediction without modifying the main task model, for more robust uncertainty quantification on regression tasks. Specifically,  our AuxUE estimates the main task prediction error and identifies Out-of-Distribution (OOD) examples. Furthermore, we propose a novel solution named Discretization-Induced Dirichlet pOsterior (DIDO), which models the Dirichlet posterior on the discretized prediction error. 

Overview of AuxUE and DIDO: Pipeline of our proposed AuxUE solution. A generalized AuxUE is considered with two DNNs σ<sub>Θ1</sub> and σ<sub>Θ2</sub> for estimating aleatoric and epistemic uncertainty, respectively. Presented notations are consistent with and described in Section 3 of the main paper. The input of AuxUE can be the input, output, or intermediate features of f, we here simplify it to the image x<sup>(i)</sup> for brevity.

![image](https://github.com/ENSTA-U2IS/DIDO/blob/main/process.png)

For more details, please refer to our [paper]((https://arxiv.org/abs/2308.09065)).

## Experiment

### Toy example
We provide a toy example for illustrating DIDO on toy dataset.

### Age estimation example
In folder `age_estimation/`, we provide the codes and instructions for DIDO applying on age estimation task. The detailed information is shown on `age_estimation/README.md`.

### Monocular depth estimation example
In folder `monocular_depth_estimation/`, we provide the codes and instructions for DIDO applying on monocular depth estimation task. The detailed information is shown on `monocular_depth_estimation/README.md`.

## TODO
1. Toy example
2. Age estimation example
3. Monocular depth estimation example

## Citation
If you find this work useful for your research, please consider citing our paper:
```
@inproceedings{yu24aaai,
  author={Xuanlong, Yu and Gianni, Franchi and Jindong, Gu and Emanuel, Aldea},
  title={Discretization-Induced Dirichlet Posterior for Robust Uncertainty Quantification on Regression},
  booktitle={The 38th Annual AAAI Conference on Artificial Intelligence},
  year={2024}
}
```
