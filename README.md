# Multi-Fidelity Literature Review List

> 💡 This is the notebook for recording MF optimization literature in preparation for the CSUR paper.
> 
>     Li K, Li F. Multi-fidelity methods for optimization: a survey[J]. arXiv preprint arXiv:2402.09638, 2024.
>
> 💡 Overview of Multi-Fidelity Optimization Software Packages are in [Multi-fidelity papers with code](https://github.com/fanli525/Multi-Fidelity-Optimization/blob/master/Multi-fidelity%20papers%20with%20code.md) 


## 1. Multi-Fidelity Surrogate Model

We provide an overview of various approaches to build a surrogate model for multi-fidelity data, with a focus on their application in MFO.


### 1.1 Single Model Methods

#### 1.1.1 Response Surface Methodology (RSM)

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 1997 | Variable-complexity response surface design of an HSCT configuration | Application: HSCT optimization | - | [PDF](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Problem%208b25a34918624e048a55e148f84b9457.md) |

#### 1.1.2 Gaussian Process (GP)

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2016 | A multi-fidelity surrogate-model-assisted evolutionary algorithm | - | - | - |
| 2  | 2016 | Multi-fidelity Gaussian Process bandit optimisation | Framework: MFBO, Model: single-GP, Fidelity: Discrete | [Matlab](https://github.com/kirthevasank/mf-gp-ucb) | [ PDF](https://www.jair.org/index.php/jair/article/view/11288) |
| 3  | 2023 | Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization | Framework: MFBO, Model: GP/MTGP, Application: Materials in pouch cells | - | - |

#### 1.1.3 Radial Basis Function (RBF)

| #  | Year | Title | Other Information | Code | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2016 | A multi-fidelity surrogate-model-assisted evolutionary algorithm | - | - | - |
| 2  | 2020 | A multi-fidelity RBF surrogate-based optimization framework | Application: Manufacturing system capacity planning | - | - |
| 3  | 2007 | Multilevel optimization strategies based on metamodel-assisted EAs | - | - | - |

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

## 1.3 Autoregressive-based (AR1) Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2022 | A multi-fidelity surrogate modeling approach for incorporating multiple non-hierarchical low-fidelity data | Model: non-hierarchical Co-Kriging, Fidelity Management: UCB/MES asynchronous batch, Discrete Fidelity, Application: Maximum Von Mises stress prediction | - | - |

## 1.4 Multi-Task Gaussian Process (MTGP) Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2023 | Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization | Framework: MFBO, Model: GP/MTGP, Fidelity Management: UCB/MES asynchronous batch, Application: Materials for optimal performance in pouch cells | [Python](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078) | [ PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 2  | 2023 | Multi-Fidelity Bayesian Optimization with Unreliable Information Sources | Framework: MFBO, Model: MTGP, Fidelity Management: MES, Continuous Fidelity: learners trees, Application: XGBoost (diabetes progression) | [Python](https://github.com/aaltopml/rmfbo) | [ PDF](https://proceedings.mlr.press/v206/mikkola23a/mikkola23a.pdf) |
| 3  | 2022 | A multi-output multi-fidelity Gaussian process model for non-hierarchical low-fidelity data fusion | - | - | - |

## 1.5 Nonlinear Hierarchical Methods

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2022 | Deep Gaussian Process-based Multi-fidelity Bayesian Optimization for Simulated Chemical Reactors | Framework: MFBO, Model: DGP, Fidelity Management: UCB, Discrete Fidelity, Application: Chemical reactor designs | [Python](https://github.com/optimal-pse-lab/pulsed-reactor-optimisation) | [ PDF](https://arxiv.org/pdf/2210.17213.pdf) |
| 2  | 2021 | Hierarchical regression framework for multi-fidelity modeling | Model: Hierarchical, Discrete Fidelity, Prediction | - | - |
| 3  | 2019 | **[IMPORTANT]** Deep Gaussian processes for multi-fidelity modeling | Model: DGP, Discrete Fidelity | [Python](https://github.com/luck1226/multisource_deepGaussianProcess) | [ PDF](https://arxiv.org/pdf/1903.07320v1.pdf) |
| 4  | 2017 | **[IMPORTANT]** Nonlinear information fusion algorithms for data-efficient multi-fidelity modeling | Model: DGP, Discrete Fidelity | [Python](https://github.com/paraklas/NARGP/tree/master) | [ PDF](https://www.researchgate.net/profile/Paris-Perdikaris-2/publication/313482464_Nonlinear_information_fusion_algorithms_for_data-efficient_multi-fidelity_modelling/links/58a0ab0baca272046aad5f88/Nonlinear-information-fusion-algorithms-for-data-efficient-multi-fidelity-modelling.pdf) |
| 5  | 2019 | **[IMPORTANT]** The Gaussian process autoregressive regression model (GPAR) | Model: DGP, Discrete Fidelity | [Python](https://github.com/wesselb/gpar) | [ PDF](https://arxiv.org/pdf/1802.07182v4.pdf) |
| 6  | 2013 | **[IMPORTANT]** Deep Gaussian Processes | Model: DGP, Discrete Fidelity | [Python](https://github.com/SheffieldML/PyDeepGP) | [ PDF](http://proceedings.mlr.press/v31/damianou13a.pdf) |
| 7  | 2017 | **[IMPORTANT]** Doubly stochastic variational inference for deep Gaussian processes | Framework: MFBO, Model: DGP, Discrete Fidelity | [Python](https://paperswithcode.com/paper/doubly-stochastic-variational-inference-for) | [ PDF](https://arxiv.org/pdf/1705.08933v2.pdf) |
| 8  | 2020 | **[IMPORTANT]** Multi-fidelity Bayesian optimization via deep neural networks | Framework: MFBO, Model: DNN, Discrete Fidelity, Fidelity Management: MES | [Python](https://www.notion.soCode-Python) | [ PDF](https://arxiv.org/pdf/2007.03117v4.pdf) |
| 9  | 2021 | **[IMPORTANT]** Batch multi-fidelity Bayesian optimization with deep auto-regressive networks | Framework: MFBO, Model: DNN, Discrete Fidelity, Fidelity Management: MES | [Python](https://github.com/shib0li/BMBO-DARN) | [ PDF](https://arxiv.org/pdf/2106.09884v2.pdf) |
| 10 | 2021 | **[IMPORTANT]** Hierarchical regression framework for multi-fidelity modeling | - | - | - |

 ## 1.6 Single GP for Continuous Fidelity

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|--------------------------|------|-----|
| 1  | 2023 | Multi-Fidelity Data-Driven Design and Analysis of Reactor and Tube Simulations | Fidelity Management: MES, Optimization, Application: Chemical reactor designs | - | - |
| 2  | 2023 | Multi-fidelity Bayesian optimization to solve the inverse Stefan problem | Fidelity Management: cfKG acquisition function, Optimization, Application: Inverse Stefan problem | - | - |

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


### 2.2 Correction-Based MFBO

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|------------------------------------------------------------|-------------------------------------------|------|-----|
| 1  | 2023 | Combining Multi-Fidelity Modelling and Asynchronous Batch Bayesian Optimization | **Framework:** MFBO, **Model:** GP/MTGP, **Fidelity Management:** UCB/MES, **Application:** Materials for pouch cells | [Code](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078) | [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 2  | 2022 | Multi-Fidelity Surrogate Model Ensemble Based on Feasible Intervals | **Model:** Kriging, **Application:** Electrode materials for pouch cells | - | - |


### 2.3 AR1-Based MFBO

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|----------------------------------------------------------|------------------|------|-----|
| 1  | 2022 | Non-Myopic Multi-Fidelity Bayesian Optimization | **Fidelity Management:** Discrete Fidelity | - | - |


### 2.4 MTGP-Based MFBO

| #  | 年份 | 题目 | 其他信息 | 代码 | PDF |
|----|------|-------------------------------------------------|---------------------------------|------|-----|
| 1  | 2022 | Supervising the Multi-Fidelity Race of Hyperparameter Configurations | **Framework:** MFBO, **Model:** Deep Kernel + GP, **Fidelity Management:** Gradually increase | [Code](https://github.com/releaunifreiburg/DyHPO) | [PDF](https://arxiv.org/pdf/2202.09774v2.pdf) |
| 2  | 2017 | Fast Bayesian Optimization of Machine Learning Hyperparameters on Large Datasets | **Framework:** MFBO, **Model:** GP, **Fidelity Management:** MES | [Code](https://github.com/automl/RoBO) | [PDF](https://arxiv.org/pdf/1605.07079v2.pdf) |
| 3  | 2017 | Multi-Fidelity Bayesian Optimization with Continuous Approximations | **Framework:** MFBO, **Model:** GP, **Fidelity Management:** MES, **Fidelity Type:** Discrete/Continuous | [Code](https://github.com/cclauss/dragonfly/tree/16071860ff2a182cf8854f11c1a7006bcae58267) | [PDF](https://arxiv.org/pdf/1703.06240v1.pdf) |
| 4  | 2020 | Practical Multi-Fidelity Bayesian Optimization for Hyperparameter Tuning | **Framework:** MFBO, **Model:** GP, **Fidelity Management:** MES, **Fidelity Type:** Discrete/Continuous | - | [PDF](https://arxiv.org/pdf/1903.04703v1.pdf) |
| 5  | 2023 | Combining Multi-Fidelity Modelling and Asynchronous Batch Bayesian Optimization | **Framework:** MFBO, **Model:** GP/MTGP, **Fidelity Management:** UCB/MES, **Application:** Materials for pouch cells | [Code](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078) | [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 6  | 2022 | A Generalized Framework of Multi-Fidelity Max-Value Entropy Search through Joint Entropy | **Framework:** MFBO, **Model:** MTGP, **Fidelity Management:** MES, **Application:** SVM, Material Data | - | - |

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

### 7.1.2 NLP (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | PASHA: Efficient HPO with Progressive Resource Allocation | xformer WMT15 German-English | Epoch | Improved Hyperband | - | [Bohdal22](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 2  | 2022 | Hyper-tune: Towards Efficient Hyper-parameter Tuning at Scale | 3-layer LSTM (Penn Treebank) | Epoch | Improved Hyperband | - | [Li22](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 3  | 2020 | A System for Massively Parallel Hyperparameter Tuning | NAS-LSTM (Penn Treebank) | Epoch | Improved Hyperband | - | [Li20](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 4  | 2022 | Supervising the Multi-fidelity Race of Hyperparameter Configurations | TaskSet (NLP tabular tasks) | Epoch | Deep Kernel + GP | Fidelity Management: Gradually Increase | [Wistuba22](https://arxiv.org/pdf/2202.09774v2.pdf) |

### 7.1.3 MLP (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | PASHA: Efficient HPO with Progressive Resource Allocation | LCBench MLP (openml-cc18) | Epoch | Improved Hyperband | - | [Bohdal22](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 2  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | FCNet (MNIST) | Epoch | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 3  | 2021 | DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization | NAS-HPO-Bench 2-layer FNN (Protein Structure, Slice Localization, Naval Propulsion, Parkinsons Telemonitoring); FNN (Adult, Letter, Higgs, MNIST, Optdigits, Poker) | Epoch | Improved Hyperband | - | [Awad21](https://arxiv.org/pdf/2105.09821v2.pdf) |
| 4  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | FNN (Adult, Letter, Higgs, MNIST, Optdigits, Poker) | Epoch | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 5  | 2022 | Supervising the Multi-fidelity Race of Hyperparameter Configurations | LCBench MLP (openml-cc18) | Epoch | Deep Kernel + GP | Fidelity Management: Gradually Increase | [Wistuba22](https://arxiv.org/pdf/2202.09774v2.pdf) |
| 6  | 2020 | Practical Multi-fidelity Bayesian Optimization for Hyperparameter Tuning | FNN (MNIST) | - | MTGP | Fidelity Management: MES, Discrete/Continuous Fidelity | [Wu20](https://arxiv.org/pdf/1903.04703v1.pdf) |

### 7.1.4 XGB (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2022 | Hyper-tune: Towards Efficient Hyper-parameter Tuning at Scale | XGBoost (Pokerhand, Covertype, Hepmass, Higgs) | Data size | Improved Hyperband | - | [Li22](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 2  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | XGBoost (Covertype) | Data size | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 3  | 2023 | Multi-Fidelity Bayesian Optimization with Unreliable Information Sources | XGBoost (diabetes progression) | Learners trees | MTGP | - | [Mikkola23](https://proceedings.mlr.press/v206/mikkola23a/mikkola23a.pdf) |

### 7.1.5 SVM (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2020 | A System for Massively Parallel Hyperparameter Tuning | SVM | - | Improved Hyperband | - | [Li20](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 2  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | MNIST | Data size | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 3  | 2017 | Fast Bayesian Optimization of ML Hyperparameters on Large Datasets | MNIST | Data size | GP | Fidelity Management: MES, Discrete Fidelity | [Klein17](https://arxiv.org/pdf/1605.07079v2.pdf) |
| 4  | 2017 | Multi-Fidelity Bayesian Optimisation with Continuous Approximations | 20 News Groups (Text Classification) | Dataset size + Training iterations | GP | Fidelity Management: MES, Discrete/Continuous Fidelity | [Kandasamy17](https://arxiv.org/pdf/1703.06240v1.pdf) |

### 7.1.6 BNN (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | Regression (Boston Housing, Protein Structure) | MCMC Steps | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 2  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | Regression (Boston Housing, Protein Structure) | MCMC Steps | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |

### 7.1.7 RL (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|------------------|---------------|------------------|----------------|-----|
| 1  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | Cartpole Benchmark | Trial Number | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 2  | 2018 | BOHB: Robust and Efficient Hyperparameter Optimization at Scale | Cartpole Benchmark | Trial Number | Improved Hyperband | - | [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf) |

### 7.1.8 AutoML (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|---------------------------------------------|---------------|------------------|----------------|-----|
| 1  | 2021 | MFES-HB: Efficient Hyperband with Multi-fidelity Quality Measurements | AutoML (MNIST, Letter, Higgs, Electricity, Kropt, Mv, Poker, Fried, A9a, 2dplanes) | Data size | Improved Hyperband | - | [Li21](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 2  | 2017 | Hyperband: Bandit-based Configuration Evaluation for Hyperparameter Optimization | Automate preprocessing & model selection (117 datasets in OpenML) | Data size | Hyperband | - | [Li17](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |

### 7.1.9 Other Classifiers (HPO in MF Optimization)

| #  | 年份  | 题目 | 任务 | Fidelity 类型 | 方法 | 其他信息 | PDF |
|----|------|------------------------------------------------------------|--------------------------------------------------|------------------|------------------|----------------|-----|
| 1  | 2017 | Hyperband: Bandit-based Configuration Evaluation for Hyperparameter Optimization | Multi-class regularized least squares classification model (CIFAR-10) | Data size | Hyperband | - | [Li17](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |

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


#### **Solver-Based Approaches**

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2017 | Multi-fidelity multi-objective efficient global optimization applied to airfoil design problems | Correction | No | Reynolds-averaged Navier–Stokes (RANS) solver, XFOIL | Airfoil optimization | - |
| 2  | 2015 | A modified variable complexity modeling for efficient multidisciplinary aircraft conceptual design | Correction | No | Aircraft Design Synthesis Program (ADSP), in-house code AADL3D | Regional jet aircraft (RJA) conceptual design, wing optimization | [Fidelity](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Fidelity%204b58f07e8ce340a89ba859499dd4cb5e.md) |
| 3  | 2004 | Multilevel variable fidelity optimization of a morphing unmanned aerial vehicle | Correction | No | FUN2D (Navier-Stokes solver), Vortex panel method | Buckle Wing optimization | [Fidelity](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Fidelity%206584c661a70646a9a2ac8f255f85c212.md) |
| 4  | 2015 | Aerodynamic response quantification of complex hypersonic configurations using variable fidelity surrogate modeling | Correction | No | Cart3D/Modified Newtonian Method | Hypersonic vehicle design | - |

### 7.2.2 Simplified Governing Equations

#### **📌 Simplified Governing Equations**
| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2013 | Research on multi-fidelity aerodynamic optimization methods | CO-Kriging | No | RANS equations, BLFP numerical method | Wing optimization | - |


#### **📌 Coarser Computational Description**
| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2000 | Optimization with Variable-Fidelity Models Applied to Wing Design | - | No | - | Wing optimization | [doi:10.2514/6.2000-841](https://arc.aiaa.org/doi/10.2514/6.2000-841) |
| 2  | 2010 | Multi-Fidelity Design Optimization of Transonic Airfoils Using Shape-Preserving Response Prediction | - | No | - | Transonic airfoil optimization | [doi:10.1016/j.jocs.2010.03.007](https://doi.org/10.1016/j.jocs.2010.03.007) |


#### **📌 Relaxed Convergence Criteria**
| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2010 | Multi-Fidelity Design Optimization of Transonic Airfoils Using Shape-Preserving Response Prediction | - | No | - | Transonic airfoil optimization | - |


#### **📌 Simulation and Experiments**
| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2019 | Application of deep learning based multi-fidelity surrogate model to robust aerodynamic design optimization | Correction, DBN | No | RANS code, real experiment | RAE 2822 airfoil, DLR-F6 wing-body model | - |
| 2  | 2016 | A multi-fidelity adaptive sampling method for metamodel-based uncertainty quantification of computer simulations | Correction | No | Hydrodynamic Solver, Fluid-Structure Interaction Solver | 3D NACA 0009 stainless steel hydrofoil | - |
| 3  | 2005 | Multi-fidelity optimization of laminated conical shells for buckling | Correction, response surfaces | No | STAGS-A, BOCS | Filament-wound laminated conical shells | - |


#### **📌 Steady/Transient**
| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2018 | Analysis of dataset selection for multi-fidelity surrogates for a turbine problem | Co-Kriging | No | Unsteady RANS solvers: Transient, TT, Steady RANS solver | Two-variable turbine problem | - |
| 2  | 2016 | High fidelity multidisciplinary design optimization of a wing using the interaction of low and high fidelity models | Correction | No | Steady Navier-Stokes equations, RANS equations | Wortmann FX60.126 2D airfoil | - |
| 3 | 1997 | Variable-complexity response surface design of an HSCT configuration | - | No | - | HSCT aerodynamic-structural optimization | [Problem](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Problem%20948b03cb331c4a468fe1594dda423e8c.md) |
| 4 | 2019 | Multi-fidelity efficient global optimization: Methodology and application to airfoil shape design | - | No | - | Airfoil shape optimization | - |

### 7.2.2 Electrode Materials

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2023 | Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization | GP/MTGP | UCB/MES asynchronous batch | Discrete Fidelity | Electrode materials for optimal performance in pouch cells | - |
### 7.2.3 Chemical Reactor Designs

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2022 | Deep Gaussian Process-based Multi-fidelity Bayesian Optimization for Simulated Chemical Reactors | DGP | UCB | Discrete Fidelity | Chemical reactor designs | [Savage22](https://arxiv.org/pdf/2210.17213.pdf) |
| 2  | 2023 | Multi-Fidelity Data-Driven Design and Analysis of Reactor and Tube Simulations | GP | MES | - | Chemical reactor designs | - |

### 7.2.4 Design Optimization

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2020 | Multi-fidelity Bayesian optimization via deep neural networks | DNN | MES | Discrete Fidelity | Mechanical Plate Vibration Design, Thermal Conductor Design | [Li20](https://arxiv.org/pdf/2007.03117v4.pdf) |
| 2  | 1991 | Combining global and local approximations | - | - | - | - | - |

### 7.2.5 Space Infrastructure

| #  | 年份  | 题目 | 方法 | Fidelity 管理 | Fidelity 级别 | 任务 | PDF |
|----|------|------------------------------------------------------------|------------------|-----------------|---------------------------------|---------------------------------|-----|
| 1  | 2021 | Multifidelity space mission planning and infrastructure design framework for space resource logistics | - | - | - | Space mission planning & infrastructure design | - |
### 7.2.6 Cooling Hold Design

| #  | 任务 | 相关文件 |
|----|-----------------|------------------------------------------------------------------------------------------------------------------|
| 1  | Cooling hold design | [Applications](MF%20literature%20review%20list%202638a7f61ad441a483611a0fc4dd21ce/Applications%20000dce3472c4448d8654a21168633612.csv) |

## 7.3 Applications in Scientific Discovery

### 7.3.1 Applications of MFO in Material Science

| #  | 年份  | 题目 | 期刊 | PDF |
|----|------|--------------------------------------------------------------|--------------------------|-----|
| 1  | 2023 | Exploring Multi-Fidelity Data in Materials Science: Challenges, Applications, and Optimized Learning Strategies | Applied Sciences | - |
| 2  | 2022 | A simple denoising approach to exploit multi-fidelity data for machine learning materials properties | npj Computational Materials | - |
| 3  | 2022 | A multi-fidelity machine learning approach to high throughput materials screening | Npj Comput. Mater. | - |
| 4  | 2023 | Accelerated Design of Architected Materials with Multifidelity Bayesian Optimization | Journal of Engineering Mechanics | - |
| 5  | 2020 | Multi-fidelity machine-learning with uncertainty quantification and Bayesian optimization for materials design: Application to ternary random alloys | The Journal of Chemical Physics | - |

### 7.3.2 Applications of MFO in Drug Discovery

| #  | 年份  | 题目 | 期刊 | 重要性 | PDF |
|----|------|--------------------------------------------------------------|--------------------------|---------|-----|
| 1  | 2023 | MF-PCBA: Multifidelity High-Throughput Screening Benchmarks for Drug Discovery and Machine Learning | Journal of Chemical Information and Modeling | **重要** | - |
| 2  | 2022 | Multi-fidelity machine learning models for improved high-throughput screening predictions | - | - | - |
| 3  | 2022 | Multi-fidelity prediction of molecular optical peaks with deep learning | Chemical Science | - | - |
| 4  | 2023 | MF-SuP-pKa: multi-fidelity modeling with subgraph pooling mechanism for pKa prediction | Acta Pharmaceutica Sinica B | **重要** | - |
| 5  | 2022 | Improving small molecule pKa prediction using transfer learning with graph neural networks | Frontiers in Chemistry | - | - |
| 6  | 2023 | Using physical property surrogate models to perform accelerated multi-fidelity optimization of force field parameters | Digital Discovery | **重要** | - |
| 7  | 2023 | Multi-Fidelity Active Learning with GFlowNets | arXiv preprint | - | - |
| 8  | 2020 | Multifidelity statistical machine learning for molecular crystal structure prediction | The Journal of Physical Chemistry A | - | - |
| 9  | 2019 | Characterizing the effect of 30 drugs on the QT interval using Gaussian process regression | Computer Methods in Applied Mechanics and Engineering | - | - |
| 10 | 2018 | Predicting the cardiac toxicity of drugs using a novel multiscale exposure–response simulator | Computer Methods in Biomechanics and Biomedical Engineering | - | - |
| 11 | 2019 | Predicting critical drug concentrations and torsadogenic risk using a multiscale exposure-response simulator | Progress in Biophysics and Molecular Biology | - | - |
| 12 | 2018 | Predicting drug‐induced arrhythmias by multiscale modeling | International Journal for Numerical Methods in Biomedical Engineering | - | - |
| 13 | 2023 | Improved GNNs for Log D 7.4 Prediction by Transferring Knowledge from Low-Fidelity Data | Journal of Chemical Information and Modeling | - | - |
| 14 | 2023 | LogD7.4 prediction enhanced by transferring knowledge from chromatographic retention time, microscopic pKa, and logP | Journal of Cheminformatics | - | - |
| 15 | 2023 | Uni-pKa: An Accurate and Physically Consistent pKa Prediction through Protonation Ensemble Modeling | - | - | - |
---

# 8. MF review paper

### 8.1 Multi-Fidelity Models

| #  | 年份  | 题目 | 期刊 |  PDF |
|----|------|--------------------------------------------------------------|--------------------------|-----|
| 1  | 2016 | Review of Multi-Fidelity Models | arXiv | [Detail](MF%20literature%20review%20list/Detail_f25d1a2c.md) |
| 2  | 2017 | Remarks on Multi-Fidelity Surrogates | Struct. Multidiscip. Optim. | [Detail](MF%20literature%20review%20list/Detail_1a2a99.md) |
| 3  | 2018 | Review of Multi-Fidelity Surrogates; When Are They Worthwhile? | - |  - |
| 4  | 2019 | Issues in Deciding Whether to Use Multi-Fidelity Surrogates | AIAA J. | [Detail](MF%20literature%20review%20list/Detail_9468b6.md) |
| 5  | 2020 | Overview of Gaussian Process Based Multi-Fidelity Techniques with Variable Relationship | Aerosp. Sci. Technol. |  [Detail](MF%20literature%20review%20list/Detail_8c072c.md) |

### 8.2 Multi-Fidelity Optimization

| #  | 年份  | 题目 | 期刊 | PDF |
|----|------|--------------------------------------------------------------|--------------------------|-----|
| 1  | 2018 | Survey of Multi-Fidelity Methods in Uncertainty Propagation, Inference, and Optimization | SIAM Rev. |  - |
| 2  | 2020 | Survey of Multi-Fidelity Surrogate Models in Engineering Design | J. Mech. Eng. | - |
| 3  | 2019 | Multi-Fidelity Approaches for Uncertainty Quantification | GAMM‐Mitteilungen |  - |

---
# 9. MF book
| #  | 年份  | 书名 | 出版社 |  链接 |
|----|------|--------------------------------------------------------------|--------------------------|----------------|
| 1  | 2023 | Multi-Fidelity Surrogates: Modeling, Optimization and Applications | Springer |  [Springer](https://link.springer.com/book/10.1007/978-981-19-7210-2) |
| 2  | 2020 | Surrogate-Model-Based Design and Optimization | Springer Singapore |  [Springer](https://link.springer.com/chapter/10.1007/978-981-15-0731-1_7) |
| 3  | 2021 | A Possibilistic Multifidelity Approach for Uncertainty Analysis | Shaker Verlag |  [Shaker Verlag](https://www.shaker.de/de/content/catalogue/index.asp?lang=de&ID=8&ISBN=978-3-8440-8034-6) |
---
# 10. MF Ph.D. Thesis

### 10.1 Multi-Fidelity Models

| #  | 年份  | 题目 | 学校 | 重要性 | PDF |
|----|------|--------------------------------------------------------------|--------------------------|---------|-----|
| 1  | 2013 | Multi-Fidelity Gaussian Process Regression for Computer Experiments | Université Paris-Diderot-Paris VII | **计算机实验** | [PDF](https://theses.hal.science/file/index/docid/866770/filename/manuscrit.pdf) |
| 2  | 2021 | Multi-Fidelity Modeling for Aerothermal Analysis | Missouri University of Science and Technology | **航天热分析** | [PDF](https://scholarsmine.mst.edu/cgi/viewcontent.cgi?article=4021&context=doctoral_dissertations) |
| 3  | 2022 | Multi-Task and Multi-Fidelity Convolutional Encoder-Decoder Networks | University of Notre Dame | **Encoder-Decoder Networks** | - |
| 4  | 2023 | Multi-Fidelity Methods for Simulation of Wax Deposition | Imperial College London | **蜡沉积模拟** | [PDF](https://spiral.imperial.ac.uk/handle/10044/1/102792) |
| 5  | 2018 | 风电场尾流场与功率多精度模拟方法研究 | 华北电力大学 | **风电场优化** | [PDF](http://cnki.cqgmy.edu.cn/KCMS/detail/detail.aspx?filename=1018241430.nh&dbcode=CDFD&dbname=CDFD2019) |


## 10.2 MF optimization

| #  | 年份  | 题目 | 学校 | 主题 | PDF |
|----|------|--------------------------------------------------------------|--------------------------|-----------------------------------|-----|
| 1  | 2007 | Surrogate-based Optimization Using Multi-Fidelity Models with Variable Parameterization | MIT | **SBO** |  [PDF](https://dspace.mit.edu/bitstream/handle/1721.1/39666/176111691-MIT.pdf?sequence=2) |
| 2  | 2012 | Multi-Fidelity Optimization for Supersonic Aircraft Design | Stanford University | **Aircraft Optimization** |  - |
| 3  | 2018 | Multi-Fidelity Multi-Objective Trust-Region-Based Optimization for High-Lift Devices | Cranfield University | **High-Lift Devices Optimization** |  [PDF](https://dspace.lib.cranfield.ac.uk/bitstream/handle/1826/17783/Demange_J_2018.pdf?sequence=1&isAllowed=y) |
| 4  | 2022 | Multi-Fidelity Methods for Uncertainty Quantification in Cardiovascular Hemodynamics | Stanford University | **Uncertainty Quantification** |  - |
| 5  | 2011 | Multidisciplinary Multi-Fidelity Optimization of Flexible Wing Aerofoils by Passive Adaptivity | University of Leeds | **Multidisciplinary Optimization of Aerofoils** | - | - |
| 6  | 2012 | Multi-Fidelity Methods for Multidisciplinary System Design | MIT | **Multidisciplinary System Design** | [PDF](https://dspace.mit.edu/bitstream/handle/1721.1/76145/820204781-MIT.pdf;sequence=2) |
| 7  | 2018 | 基于多保真度建模的多层级筒壳屈曲分析及优化方法研究 | 大连理工大学 | **多层级筒壳屈曲分析及优化** |  - |
| 8  | 2022 | 基于变可信度近似模型的序贯稳健性优化设计方法研究 | 华中科技大学 | **稳健性优化** |  - |
| 9  | 2020 | 多精度数据驱动的昂贵优化问题求解及其在天线设计中的应用 | 中国地质大学 | **天线设计** |  - |

---

# 11. MF report

| #  | 年份  | 题目 | 机构 | 主题 | PDF |
|----|------|--------------------------------------------------------------|-------------------------------|--------------------------------------|-----|
| 1  | 2003 | On Developing a Multifidelity Modeling Algorithm for System-Level Engineering Analysis | Sandia National Lab (SNL) | **System-Level Engineering Analysis** | [PDF](https://web.archive.org/web/20161227025614id_/http://prod.sandia.gov/techlib/access-control.cgi/2003/030399.pdf) |
| 2  | 2010 | Multifidelity Analysis and Optimization for Supersonic Design | NASA | **Supersonic Design** | [PDF](https://ntrs.nasa.gov/api/citations/20100042294/downloads/20100042294.pdf) |
| 3  | 2021 | Multifidelity Monte Carlo Estimators for Robust Formulations in Optimization under Uncertainty | Sandia National Lab (SNL) | **Optimization under Uncertainty** | [PDF](https://www.osti.gov/servlets/purl/1847580) |
| 4  | 2017 | Multilevel-Multifidelity Approaches for Uncertainty Quantification and Design | Sandia National Lab (SNL) | **Uncertainty Quantification** | [PDF](https://www.osti.gov/servlets/purl/1455372) |
| 5  | 2019 | Recent Advancement in Multifidelity Uncertainty Quantification | Sandia National Lab (SNL) | **Uncertainty Quantification** | [PDF](https://www.osti.gov/servlets/purl/1642820) |

