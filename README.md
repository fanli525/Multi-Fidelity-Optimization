# Multi-Fidelity Literature Review List

> 💡 This is the notebook for recording MF optimization literature in preparation for the CSUR paper.

---

## 1. Multi-Fidelity Surrogate Model

We provide an overview of various approaches to build a surrogate model for multi-fidelity data, with a focus on their application in MFO.

---

### 1.1 Single Model Methods

#### 1.1.1 Response Surface Methodology (RSM)

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 1997 | Variable-complexity response surface design of an HSCT configuration | Application: HSCT optimization | - | [📄 Link](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Problem%208b25a34918624e048a55e148f84b9457.md) |

#### 1.1.2 Gaussian Process (GP)

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2016 | A multi-fidelity surrogate-model-assisted evolutionary algorithm | - | - | - |
| 2  | 2016 | Multi-fidelity Gaussian Process bandit optimisation | Framework: MFBO, Model: single-GP, Fidelity: Discrete | [💻 Matlab](https://github.com/kirthevasank/mf-gp-ucb) | [📄 PDF](https://www.jair.org/index.php/jair/article/view/11288) |
| 3  | 2023 | Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization | Framework: MFBO, Model: GP/MTGP, Application: Materials in pouch cells | - | - |

#### 1.1.3 Radial Basis Function (RBF)

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2016 | A multi-fidelity surrogate-model-assisted evolutionary algorithm | - | - | - |
| 2  | 2020 | A multi-fidelity RBF surrogate-based optimization framework | Application: Manufacturing system capacity planning | - | - |
| 3  | 2007 | Multilevel optimization strategies based on metamodel-assisted EAs | - | - | - |

---

### 1.2 Correction-Based Methods

#### 1.2.1 First-Order Taylor Series

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 1991 | Combining global and local approximations | - | - | - |
| 2  | 1993 | Sensitivity-based scaling for approximating structural response | - | - | - |
| 3  | 2000 | A multigrid approach to the optimization of systems governed by differential equations | - | - | - |

#### 1.2.2 Second-Order Taylor Series

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2004 | Second-order corrections for surrogate-based optimization with model hierarchies | - | - | - |
| 2  | 2004 | Multilevel variable fidelity optimization of a morphing UAV | - | - | - |

---

## 1.3 Autoregressive-based (AR1) Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2022 | A multi-fidelity surrogate modeling approach for incorporating multiple non-hierarchical low-fidelity data | Model: non-hierarchical Co-Kriging, Fidelity Management: UCB/MES asynchronous batch, Discrete Fidelity, Application: Maximum Von Mises stress prediction | - | - |

---

## 1.4 Multi-Task Gaussian Process (MTGP) Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2023 | Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization | Framework: MFBO, Model: GP/MTGP, Fidelity Management: UCB/MES asynchronous batch, Application: Materials for optimal performance in pouch cells | [💻 Python](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078) | [📄 PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 2  | 2023 | Multi-Fidelity Bayesian Optimization with Unreliable Information Sources | Framework: MFBO, Model: MTGP, Fidelity Management: MES, Continuous Fidelity: learners trees, Application: XGBoost (diabetes progression) | [💻 Python](https://github.com/aaltopml/rmfbo) | [📄 PDF](https://proceedings.mlr.press/v206/mikkola23a/mikkola23a.pdf) |
| 3  | 2022 | A multi-output multi-fidelity Gaussian process model for non-hierarchical low-fidelity data fusion | - | - | - |

---## 1.5 Nonlinear Hierarchical Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2022 | Deep Gaussian Process-based Multi-fidelity Bayesian Optimization for Simulated Chemical Reactors | Framework: MFBO, Model: DGP, Fidelity Management: UCB, Discrete Fidelity, Application: Chemical reactor designs | [💻 Python](https://github.com/optimal-pse-lab/pulsed-reactor-optimisation) | [📄 PDF](https://arxiv.org/pdf/2210.17213.pdf) |
| 2  | 2021 | Hierarchical regression framework for multi-fidelity modeling | Model: Hierarchical, Discrete Fidelity, Prediction | - | - |
| 3  | 2019 | **[IMPORTANT]** Deep Gaussian processes for multi-fidelity modeling | Model: DGP, Discrete Fidelity | [💻 Python](https://github.com/luck1226/multisource_deepGaussianProcess) | [📄 PDF](https://arxiv.org/pdf/1903.07320v1.pdf) |
| 4  | 2017 | **[IMPORTANT]** Nonlinear information fusion algorithms for data-efficient multi-fidelity modeling | Model: DGP, Discrete Fidelity | [💻 Python](https://github.com/paraklas/NARGP/tree/master) | [📄 PDF](https://www.researchgate.net/profile/Paris-Perdikaris-2/publication/313482464_Nonlinear_information_fusion_algorithms_for_data-efficient_multi-fidelity_modelling/links/58a0ab0baca272046aad5f88/Nonlinear-information-fusion-algorithms-for-data-efficient-multi-fidelity-modelling.pdf) |
| 5  | 2019 | **[IMPORTANT]** The Gaussian process autoregressive regression model (GPAR) | Model: DGP, Discrete Fidelity | [💻 Python](https://github.com/wesselb/gpar) | [📄 PDF](https://arxiv.org/pdf/1802.07182v4.pdf) |
| 6  | 2013 | **[IMPORTANT]** Deep Gaussian Processes | Model: DGP, Discrete Fidelity | [💻 Python](https://github.com/SheffieldML/PyDeepGP) | [📄 PDF](http://proceedings.mlr.press/v31/damianou13a.pdf) |
| 7  | 2017 | **[IMPORTANT]** Doubly stochastic variational inference for deep Gaussian processes | Framework: MFBO, Model: DGP, Discrete Fidelity | [💻 Python](https://paperswithcode.com/paper/doubly-stochastic-variational-inference-for) | [📄 PDF](https://arxiv.org/pdf/1705.08933v2.pdf) |
| 8  | 2020 | **[IMPORTANT]** Multi-fidelity Bayesian optimization via deep neural networks | Framework: MFBO, Model: DNN, Discrete Fidelity, Fidelity Management: MES | [💻 Python](https://www.notion.soCode-Python) | [📄 PDF](https://arxiv.org/pdf/2007.03117v4.pdf) |
| 9  | 2021 | **[IMPORTANT]** Batch multi-fidelity Bayesian optimization with deep auto-regressive networks | Framework: MFBO, Model: DNN, Discrete Fidelity, Fidelity Management: MES | [💻 Python](https://github.com/shib0li/BMBO-DARN) | [📄 PDF](https://arxiv.org/pdf/2106.09884v2.pdf) |
| 10 | 2021 | **[IMPORTANT]** Hierarchical regression framework for multi-fidelity modeling | - | - | - |

---

 ## 1.6 Single GP for Continuous Fidelity

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2023 | Multi-Fidelity Data-Driven Design and Analysis of Reactor and Tube Simulations | Fidelity Management: MES, Optimization, Application: Chemical reactor designs | - | - |
| 2  | 2023 | Multi-fidelity Bayesian optimization to solve the inverse Stefan problem | Fidelity Management: cfKG acquisition function, Optimization, Application: Inverse Stefan problem | - | - |

---
## 1.7 Space Mapping Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 1994 | **[IMPORTANT]** Space mapping technique for electromagnetic optimization | Cited by 833 | - | - |
| 2  | 1995 | **[IMPORTANT]** Electromagnetic Optimization Exploiting Aggressive Space Mapping | Aggressive space mapping, Cited by 482 | - | - |
| 3  | 1996 | Fully Automated Space Mapping Optimization of 3D Structures | Cited by 57 | - | - |
| 4  | 1998 | **[IMPORTANT]** A trust region aggressive space mapping algorithm for EM optimization | Trust regions, Cited by 177 | - | - |
| 5  | 1999 | A hybrid aggressive space-mapping algorithm for EM optimization | Trust regions, Cited by 134 | - | - |
| 6  | 2005 | **[IMPORTANT-SANDIA REPORT]** Developing a computationally efficient dynamic multilevel hybrid optimization scheme | Tech report, Sandia National Laboratories, Cited by 17 | - | - |
| 7  | 2000 | Neural space mapping EM optimization of microwave structures | Artificial neural networks, Cited by 26 | - | - |
| 8  | 2008 | **[IMPORTANT]** Surrogate-based optimization using multifidelity models with variable parameterization and corrected space mapping | Cited by 278 | - | - |
| 9  | 2015 | Shape Optimization of Trawl-doors Using Variable-fidelity Models and Space Mapping | Cited by 27 | - | - |
| 10 | 2016 | **[Manifold Mapping]** Multi-Fidelity Aerodynamic Shape Optimization Using Manifold Mapping | Cited by 15 | - | - |
| 11 | 2016 | Rapid Multi-Objective Aerodynamic Design Using Co-Kriging and Space Mapping | Not important, Cited by 20 | - | - |
| 12 | 2004 | Convergence of Hybrid Space Mapping Algorithms | Cited by 29 | - | - |
| 13 | 2004 | Implicit space mapping optimization exploiting preassigned parameters | Implicit space mapping | - | - |
| 14 | 2005 | Efficient analytical formulation and sensitivity analysis of neuro-space mapping for nonlinear microwave device modeling | Neural-based space mapping | - | - |
| 15 | 2008 | Statistical neuro-space mapping technique for large-signal modeling of nonlinear devices | Neural-based space mapping | - | - |
| 16 | 2005 | A linear inverse space-mapping (LISM) algorithm for designing linear and nonlinear RF and microwave circuits | Inverse problems | - | - |
| 17 | 2009 | Accelerated microwave design optimization with tuning space mapping | Tuning space mapping | - | - |

---

> 📌 This section provides an overview of **space mapping methods** in multi-fidelity optimization, including **trust regions, aggressive space mapping, neural-based space mapping**, and **manifold mapping**.


