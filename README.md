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

## 2. Bayesian Optimization for MFO

### 2.1 Single Model-Based MFBO
(无文献记录)

---

### 2.2 Correction-Based MFBO

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|------|-----|
| 1  | 2023 | Combining Multi-Fidelity Modelling and Asynchronous Batch Bayesian Optimization | **Framework:** MFBO, **Model:** GP/MTGP, **Fidelity Management:** UCB/MES, **Application:** Materials for pouch cells | [Code](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078) | [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 2  | 2022 | Multi-Fidelity Surrogate Model Ensemble Based on Feasible Intervals | **Model:** Kriging, **Application:** Electrode materials for pouch cells | - | - |

---

### 2.3 AR1-Based MFBO

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|----------------------------------------------------------|------------------|------|-----|
| 1  | 2022 | Non-Myopic Multi-Fidelity Bayesian Optimization | **Fidelity Management:** Discrete Fidelity | - | - |

---

### 2.4 MTGP-Based MFBO

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|---------------------------------|------|-----|
| 1  | 2022 | Supervising the Multi-Fidelity Race of Hyperparameter Configurations | **Framework:** MFBO, **Model:** Deep Kernel + GP, **Fidelity Management:** Gradually increase | [Code](https://github.com/releaunifreiburg/DyHPO) | [PDF](https://arxiv.org/pdf/2202.09774v2.pdf) |
| 2  | 2017 | Fast Bayesian Optimization of Machine Learning Hyperparameters on Large Datasets | **Framework:** MFBO, **Model:** GP, **Fidelity Management:** MES | [Code](https://github.com/automl/RoBO) | [PDF](https://arxiv.org/pdf/1605.07079v2.pdf) |
| 3  | 2017 | Multi-Fidelity Bayesian Optimization with Continuous Approximations | **Framework:** MFBO, **Model:** GP, **Fidelity Management:** MES, **Fidelity Type:** Discrete/Continuous | [Code](https://github.com/cclauss/dragonfly/tree/16071860ff2a182cf8854f11c1a7006bcae58267) | [PDF](https://arxiv.org/pdf/1703.06240v1.pdf) |
| 4  | 2020 | Practical Multi-Fidelity Bayesian Optimization for Hyperparameter Tuning | **Framework:** MFBO, **Model:** GP, **Fidelity Management:** MES, **Fidelity Type:** Discrete/Continuous | - | [PDF](https://arxiv.org/pdf/1903.04703v1.pdf) |
| 5  | 2023 | Combining Multi-Fidelity Modelling and Asynchronous Batch Bayesian Optimization | **Framework:** MFBO, **Model:** GP/MTGP, **Fidelity Management:** UCB/MES, **Application:** Materials for pouch cells | [Code](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078) | [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 6  | 2022 | A Generalized Framework of Multi-Fidelity Max-Value Entropy Search through Joint Entropy | **Framework:** MFBO, **Model:** MTGP, **Fidelity Management:** MES, **Application:** SVM, Material Data | - | - |

---

### 2.5 Nonlinear Hierarchical-Based MFBO

| #  | 年份  | 题目 | 其他信息 | 代码 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|------|-----|
| 1  | 2020 | Multi-Fidelity Bayesian Optimization via Deep Neural Networks | **Framework:** MFBO, **Model:** DNN, **Fidelity Management:** MES, **Fidelity Type:** Discrete | [Code](https://www.notion.soCode-Python) | [PDF](https://arxiv.org/pdf/2007.03117v4.pdf) |
| 2  | 2021 | Batch Multi-Fidelity Bayesian Optimization with Deep Auto-Regressive Networks | **Framework:** MFBO, **Model:** DNN, **Fidelity Management:** MES, **Fidelity Type:** Discrete | [Code](https://github.com/shib0li/BMBO-DARN) | [PDF](https://arxiv.org/pdf/2106.09884v2.pdf) |
| 3  | 2022 | Deep Gaussian Process-Based Multi-Fidelity Bayesian Optimization for Simulated Chemical Reactors | **Framework:** MFBO, **Model:** DGP, **Fidelity Management:** UCB, **Fidelity Type:** Discrete, **Application:** Chemical reactor designs | [Code](https://github.com/optimal-pse-lab/pulsed-reactor-optimisation) | [PDF](https://arxiv.org/pdf/2210.17213.pdf) |

---
### 3. Surrogate-Assisted EAs for MFO

| #  | 年份  | 题目 | 其他信息 | 代码 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|------|-----|
| 1  | 2020 | A Multi-Fidelity RBF Surrogate-Based Optimization Framework for Computationally Expensive Multi-Modal Problems | **Optimization**, **Application:** Capacity planning for manufacturing systems | - | - |
| 2  | 2022 | An Iterative Two-Stage Multi-Fidelity Optimization Algorithm for Computationally Expensive Problems | - | - | - |
| 3  | 2023 | A Test Suite for Multi-Objective Multi-Fidelity Optimization | **Conference:** EMO’23 | [Code](http://www.mdolab.net/research_resources.html) | [PDF](https://link.springer.com/chapter/10.1007/978-3-031-27250-9_26) |

---
### 4. Bandit-Based MF Algorithm

| #  | 年份  | 题目 | 其他信息 | 代码 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|------|-----|
| 1  | 2013 | Almost Optimal Exploration in Multi-Armed Bandits | **Conference:** PMLR'13 | - | - |
| 2  | 2016 | Non-Stochastic Best Arm Identification and Hyperparameter Optimization | **Framework:** Bandit, **Model:** No, **Fidelity:** Discrete | [Code](https://github.com/mlr-org/mlr3hyperband) | [PDF](https://arxiv.org/pdf/1502.07943v1.pdf) |
| 3  | 2017 | Hyperband: Bandit-Based Configuration Evaluation for Hyperparameter Optimization | **Framework:** Bandit, **Model:** No, **Fidelity:** Discrete | [Code](https://github.com/automl/HpBandSter) | [PDF](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |
| 4  | 2017 | Hyperparameter Optimization of Deep Neural Networks: Combining Hyperband with Bayesian Model Selection | **Conference:** CAp'17 | - | - |
| 5  | 2018 | Combination of Hyperband and Bayesian Optimization for Hyperparameter Optimization in Deep Learning | **Conference:** arXiv | - | - |
| 6  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | **Framework:** Bandit, **Model:** TPE, **Fidelity:** Discrete | [Code](https://github.com/automl/HpBandSter) | [PDF](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 7  | 2020 | A System for Massively Parallel Hyperparameter Tuning | **Framework:** Bandit, **Model:** No, **Fidelity:** Discrete | [Code](https://paperswithcode.com/paper/massively-parallel-hyperparameter-tuning) | [PDF](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 8  | 2021 | DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization | **Framework:** Bandit, **Model:** No, **Fidelity:** Discrete | [Code](https://paperswithcode.com/paper/dehb-evolutionary-hyberband-for-scalable) | [PDF](https://arxiv.org/pdf/2105.09821v2.pdf) |
| 9  | 2021 | MFES-HB: Efficient Hyperband with Multi-Fidelity Quality Measurements | **Framework:** Bandit, **Model:** Random Forest, **Fidelity:** Discrete | [Code](https://paperswithcode.com/paper/mfes-hb-efficient-hyperband-with-multi) | [PDF](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 10 | 2022 | Hyper-Tune: Towards Efficient Hyper-Parameter Tuning at Scale | **Framework:** Bandit, **Model:** Random Forest, **Fidelity:** Discrete | [Code](https://github.com/thomas-young-2013/HyperTune) | [PDF](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 11 | 2022 | PASHA: Efficient HPO with Progressive Resource Allocation | **Framework:** Bandit, **Model:** No, **Fidelity:** Discrete | [Code](https://paperswithcode.com/paper/pasha-efficient-hpo-with-progressive-resource) | [PDF](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 12 | 2022 | GPTuneBand: Multi-Task and Multi-Fidelity Autotuning for Large-Scale HPC Applications | **Framework:** Bandit, **Model:** LMC, **Fidelity:** Discrete | [Code](https://github.com/gptune/GPTune) | [PDF](https://crd.lbl.gov/assets/Uploads/GPTuneBand.pdf) |

---
### 6. Benchmark Problems in MFO

#### 6.1 Synthetic Problems

| #  | 年份  | 题目 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|-----|
| 1  | 2023 | A Test Suite for Multi-objective Multi-fidelity Optimization | **Conference:** EMO’23 | - |
| 2  | 2022 | Bifidelity Surrogate Modelling: Showcasing the Need for New Test Instances | **Journal:** INFORMS Journal on Computing | - |

#### 6.2 NAS Benchmark

| #  | 年份  | 题目 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|-----|
| 1  | 2018 | DARTS: Differentiable Architecture Search | **Conference:** ICML’18, **Cited by:** 3813 | - |
| 2  | 2019 | Nas-bench-101: Towards Reproducible Neural Architecture Search | **Conference:** ICML’19, **Cited by:** 504 | - |
| 3  | 2019 | NAS-Bench-201: Extending the Scope of Reproducible Neural Architecture Search | **Conference:** ICML’19, **Cited by:** 530 | - |
| 4  | 2021 | Pre-trained Gaussian Processes for Bayesian Optimization | **arXiv**, **Cited by:** 9 **(xformer)** | - |

---
### 7.1.1 CNN (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | PASHA: Efficient HPO with Progressive Resource Allocation | NASBench201 (CIFAR-10, CIFAR-100, ImageNet16-120); ResNet50 (ImageNet) | Epoch | Improved Hyperband | - | [Bohdal22](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 2  | 2022 | Hyper-tune: Towards Efficient Hyper-parameter Tuning at Scale | NASBench201 (CIFAR-10, CIFAR-100, ImageNet16-120); ResNet (CIFAR-10) | Epoch | Improved Hyperband | - | [Li22](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 3  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | ResNet50 (CIFAR-10) | Epoch | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 4  | 2021 | DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization | NAS-Bench-101 (CIFAR-10); NASBench-1shot1 (CIFAR-10); NASBench201 (CIFAR-10, CIFAR-100, ImageNet16-120); ResNet50 (ImageNet) | Epoch | Improved Hyperband | - | [Awad21](https://arxiv.org/pdf/2105.09821v2.pdf) |
| 5  | 2020 | A System for Massively Parallel Hyperparameter Tuning | NAS-Bench-Darts (CIFAR-10); Small CNN (CIFAR-10) | Epoch | Improved Hyperband | - | [Li20](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 6  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | Medium-Sized Small CNN (CIFAR-10) | Epoch | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 7  | 2018 | Combination of Hyperband and Bayesian Optimization for Hyperparameter Optimization in Deep Learning | LeNet (MNIST); AlexNet (CIFAR-10, MRBI, SVHN) | Num of Training Images | BO + Hyperband | - | [Wang18](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 8  | 2017 | Hyperparameter Optimization of Deep Neural Networks: Combining Hyperband with Bayesian Model Selection | CNN (MNIST) | Epoch | BO + Hyperband | - | [Bertrand17](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 9  | 2017 | Hyperband: Bandit-based Configuration Evaluation for Hyperparameter Optimization | CNN (CIFAR-10, Rotated MNIST, SVHN) | Epoch | Hyperband | - | [Li17](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |
| 10 | 2022 | Supervising the Multi-fidelity Race of Hyperparameter Configurations | NASBench201 (CIFAR-10, CIFAR-100, ImageNet16-120) | Epoch | Deep Kernel + GP | Fidelity Management: Gradually Increase | [Wistuba22](https://arxiv.org/pdf/2202.09774v2.pdf) |
| 11 | 2017 | Fast Bayesian Optimization of ML Hyperparameters on Large Datasets | CNN with 3 Conv Layers (CIFAR-10, SVHN); ResNet (CIFAR-10) | Data Size | GP | Fidelity Management: MES, Discrete Fidelity | [Klein17](https://arxiv.org/pdf/1605.07079v2.pdf) |
| 12 | 2020 | Practical Multi-fidelity Bayesian Optimization for Hyperparameter Tuning | CNN with 3 Conv Layers (CIFAR-10, SVHN) | Data Size + Epoch | MTGP | Fidelity Management: MES, Discrete/Continuous Fidelity | [Wu20](https://arxiv.org/pdf/1903.04703v1.pdf) |
| 13 | 2022 | Accelerating Evolutionary Neural Architecture Search via Multifidelity Evaluation | NAS (CIFAR-10, CIFAR-100, ImageNet16-120) | Epoch + Epoch | - | Fidelity Management: Gradually Increase, Continuous Fidelity | - |

---
### 7.1.2 NLP (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | PASHA: Efficient HPO with Progressive Resource Allocation | xformer WMT15 German-English | Epoch | Improved Hyperband | - | [Bohdal22](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 2  | 2022 | Hyper-tune: Towards Efficient Hyper-parameter Tuning at Scale | 3-layer LSTM (Penn Treebank) | Epoch | Improved Hyperband | - | [Li22](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 3  | 2020 | A System for Massively Parallel Hyperparameter Tuning | NAS-LSTM (Penn Treebank) | Epoch | Improved Hyperband | - | [Li20](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 4  | 2022 | Supervising the Multi-fidelity Race of Hyperparameter Configurations | TaskSet (NLP tabular tasks) | Epoch | Deep Kernel + GP | Fidelity Management: Gradually Increase | [Wistuba22](https://arxiv.org/pdf/2202.09774v2.pdf) |

---### 7.1.3 MLP (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | PASHA: Efficient HPO with Progressive Resource Allocation | LCBench MLP (openml-cc18) | Epoch | Improved Hyperband | - | [Bohdal22](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 2  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | FCNet (MNIST) | Epoch | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 3  | 2021 | DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization | NAS-HPO-Bench 2-layer FNN (Protein Structure, Slice Localization, Naval Propulsion, Parkinsons Telemonitoring); FNN (Adult, Letter, Higgs, MNIST, Optdigits, Poker) | Epoch | Improved Hyperband | - | [Awad21](https://arxiv.org/pdf/2105.09821v2.pdf) |
| 4  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | FNN (Adult, Letter, Higgs, MNIST, Optdigits, Poker) | Epoch | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 5  | 2022 | Supervising the Multi-fidelity Race of Hyperparameter Configurations | LCBench MLP (openml-cc18) | Epoch | Deep Kernel + GP | Fidelity Management: Gradually Increase | [Wistuba22](https://arxiv.org/pdf/2202.09774v2.pdf) |
| 6  | 2020 | Practical Multi-fidelity Bayesian Optimization for Hyperparameter Tuning | FNN (MNIST) | - | MTGP | Fidelity Management: MES, Discrete/Continuous Fidelity | [Wu20](https://arxiv.org/pdf/1903.04703v1.pdf) |

---### 7.1.4 XGB (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | Hyper-tune: Towards Efficient Hyper-parameter Tuning at Scale | XGBoost (Pokerhand, Covertype, Hepmass, Higgs) | Data size | Improved Hyperband | - | [Li22](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 2  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | XGBoost (Covertype) | Data size | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 3  | 2023 | Multi-Fidelity Bayesian Optimization with Unreliable Information Sources | XGBoost (diabetes progression) | Learners trees | MTGP | - | [Mikkola23](https://proceedings.mlr.press/v206/mikkola23a/mikkola23a.pdf) |

---### 7.1.5 SVM (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2020 | A System for Massively Parallel Hyperparameter Tuning | SVM | - | Improved Hyperband | - | [Li20](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 2  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | MNIST | Data size | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 3  | 2017 | Fast Bayesian Optimization of ML Hyperparameters on Large Datasets | MNIST | Data size | GP | Fidelity Management: MES, Discrete Fidelity | [Klein17](https://arxiv.org/pdf/1605.07079v2.pdf) |
| 4  | 2017 | Multi-Fidelity Bayesian Optimisation with Continuous Approximations | 20 News Groups (Text Classification) | Dataset size + Training iterations | GP | Fidelity Management: MES, Discrete/Continuous Fidelity | [Kandasamy17](https://arxiv.org/pdf/1703.06240v1.pdf) |

---### 7.1.6 BNN (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | Regression (Boston Housing, Protein Structure) | MCMC Steps | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 2  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | Regression (Boston Housing, Protein Structure) | MCMC Steps | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |

---### 7.1.7 RL (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|------------------|---------------|------------------|----------------|-----|
| 1  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | Cartpole Benchmark | Trial Number | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 2  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | Cartpole Benchmark | Trial Number | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |

---

### 7.1.8 AutoML (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|---------------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | AutoML (MNIST, Letter, Higgs, Electricity, Kropt, Mv, Poker, Fried, A9a, 2dplanes) | Data size | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 2  | 2017 | Hyperband: Bandit-based Configuration Evaluation for Hyperparameter Optimization | Automate preprocessing & model selection (117 datasets in OpenML) | Data size | Hyperband | - | [Li17](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |

---
### 7.1.9 Other Classifiers (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------------------|------------------|------------------|----------------|-----|
| 1  | 2017 | Hyperband: Bandit-based Configuration Evaluation for Hyperparameter Optimization | Multi-class regularized least squares classification model (CIFAR-10) | Data size | Hyperband | - | [Li17](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |

---
### 7.1.10 PINN (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------------------|------------------|------------------|----------------|-----|
| 1  | 2022 | Multifidelity Modeling for Physics-Informed Neural Networks (PINNs) | PINN | Width, depth, and optimization criteria | - | - | [Penwarden22](https://www.sciencedirect.com/science/article/abs/pii/S002199912200650X) |
| 2  | 2022 | Physics-Informed Multi-Fidelity Learning-Driven Imaging Method for Electrical Capacitance Tomography | Reconstructing high-accuracy tomograms | Image model fidelity | - | - | [Lei22](https://www.sciencedirect.com/science/article/pii/S0952197622001463) |

---
## 7.2 Engineering

### 7.2.1 Aircraft Optimization

#### **Fidelity Setting**

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2008 | A multifidelity gradient-free optimization method and application to aerodynamic design | Correction/GP | No | 3D panel method / Area-rule | Axisymmetric Bodies With Low Wave Drag | - |
| 2  | 2014 | Multifidelity multidisciplinary whole-engine thermomechanical design optimization | Co-Kriging | No | 2D transient thermo-mechanical simulations or 3D mechanical simulations | Engine optimization | - |
| 3  | 2012 | Constrained multifidelity optimization using model calibration | Correction, trust region | No | Cart3D/Linearized panel | Supersonic airfoil design | - |
| 4  | 2019 | Input mapping for model calibration with application to wing aerodynamics | Correction | No | Thin-surface Vortex Lattice Method (VLM), Thick-surface Vortex Ring Method (VRM) | Wing optimization | - |
| 5  | 2017 | Enhanced multi-fidelity model for flight simulation using global exploration and the Kriging method | Correction, Kriging | No | AVL, AADL-3D | Wing optimization | - |

---

#### **Solver-Based Approaches**

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2017 | Multi-fidelity multi-objective efficient global optimization applied to airfoil design problems | Correction | No | Reynolds-averaged Navier–Stokes (RANS) solver, XFOIL | Airfoil optimization | - |
| 2  | 2015 | A modified variable complexity modeling for efficient multidisciplinary aircraft conceptual design | Correction | No | Aircraft Design Synthesis Program (ADSP), in-house code AADL3D | Regional jet aircraft (RJA) conceptual design, wing optimization | [Fidelity](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Fidelity%204b58f07e8ce340a89ba859499dd4cb5e.md) |
| 3  | 2004 | Multilevel variable fidelity optimization of a morphing unmanned aerial vehicle | Correction | No | FUN2D (Navier-Stokes solver), Vortex panel method | Buckle Wing optimization | [Fidelity](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Fidelity%206584c661a70646a9a2ac8f255f85c212.md) |
| 4  | 2015 | Aerodynamic response quantification of complex hypersonic configurations using variable fidelity surrogate modeling | Correction | No | Cart3D/Modified Newtonian Method | Hypersonic vehicle design | - |

---






