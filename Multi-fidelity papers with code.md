# Multi-fidelity Papers with Code

💡 This is the notebook for recording MF optimization literature in preparation for the CSUR paper.

## 1. Bayesian Optimization for MFO

### 1.1 Single model-based MFBO

| #  | Paper | Framework | Model | Fidelity Management | Fidelity Type | Code | PDF |
|----|---------------------------------------------|------------|------|-------------------|--------------|----|----|
| 1  | Kandasamy et al., 2016, *J. Artif. Intell. Res.* (cited by 75) | MFBO | Single Model-GP | UCB | Discrete Fidelity | [Matlab](https://github.com/kirthevasank/mf-gp-ucb) | [PDF](https://www.jair.org/index.php/jair/article/view/11288) |

### 1.2 Correction-based MFBO

| #  | Paper | Framework | Model | Fidelity Management | Fidelity Type | Application | Code | PDF |
|----|---------------------------------------------|------------|------|-------------------|--------------|--------------|----|----|
| 1  | Folch et al., 2023, *Comput. Chem. Eng.* (cited by 7) | MFBO | GP/MTGP | UCB/MES asynchronous batch | Discrete Fidelity | Materials for pouch cells | [Python](https://github.com/jpfolch/MFBoom) | [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |

### 1.3 MTGP-based MFBO

| #  | Paper | Framework | Model | Fidelity Management | Fidelity Type | Application | Code | PDF |
|----|---------------------------------------------|------------|------|-------------------|--------------|--------------|----|----|
| 1  | Wistuba et al., 2022, *NeurIPS* (cited by 3) | MFBO | Deep Kernel+GP | Gradually Increase | Discrete Fidelity | - | [Python](https://github.com/releaunifreiburg/DyHPO) | [PDF](https://arxiv.org/pdf/2202.09774v2.pdf) |
| 2  | Klein et al., 2017, *AISTATS* (cited by 592) | MFBO | GP | MES | Discrete Fidelity | - | [Python](https://github.com/automl/RoBO) | [PDF](https://arxiv.org/pdf/1605.07079v2.pdf) |
| 3  | Kandasamy et al., 2017, *ICML* (cited by 201) | MFBO | GP | MES | Discrete/Continuous Fidelity | - | [Python](https://github.com/cclauss/dragonfly) | [PDF](https://arxiv.org/pdf/1703.06240v1.pdf) |
| 4  | Wu et al., 2020, *UAI* (cited by 113) | MFBO | GP | MES | Discrete/Continuous Fidelity | - | - | [PDF](https://arxiv.org/pdf/1903.04703v1.pdf) |
| 5  | Folch et al., 2023, *Comput. Chem. Eng.* (cited by 7) | MFBO | GP/MTGP | UCB/MES asynchronous batch | Discrete Fidelity | Materials for pouch cells | [Python](https://www.notion.so/colalab/MF-literature-review-list) | [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637) |
| 6  | Takeno et al., 2022, *Neural Comput.* (cited by 4) | MFBO | MTGP | MES | Discrete Fidelity | SVM, Material Data | [Python](https://github.com/takeuchi-lab/MF-MES) | [PDF](https://watermark.silverchair.com/neco_a_01530.pdf) |
| 7  | Mikkola et al., 2023, *AISTATS* (cited by 1) | MFBO | MTGP | MES | Continuous Fidelity | XGBoost (Diabetes Progression) | [Python](https://github.com/aaltopml/rmfbo) | [PDF](https://proceedings.mlr.press/v206/mikkola23a/mikkola23a.pdf) |

### 1.4 Nonlinear Hierarchical-based MFBO

| #  | Paper | Framework | Model | Fidelity Management | Fidelity Type | Application | Code | PDF |
|----|---------------------------------------------|------------|------|-------------------|--------------|--------------|----|----|
| 1  | Li et al., 2020, *NeurIPS* (cited by 33) | MFBO | DNN | MES | Discrete Fidelity | - | [Python](https://github.com/shib0li/DNN-MFBO) | [PDF](https://arxiv.org/pdf/2007.03117v4.pdf) |
| 2  | Li et al., 2021, *NeurIPS* (cited by 33) | MFBO | DNN | MES | Discrete Fidelity | - | [Python](https://github.com/shib0li/BMBO-DARN) | [PDF](https://arxiv.org/pdf/2106.09884v2.pdf) |
| 3  | Savage et al., 2022, *NeurIPS* (cited by 3) | MFBO | DGP | UCB | Discrete Fidelity | Chemical Reactor Designs | [Python](https://github.com/optimal-pse-lab/pulsed-reactor-optimisation) | [PDF](https://arxiv.org/pdf/2210.17213.pdf) |
| 4  | Cutajar et al., 2019, *arXiv* (cited by 94) | MFBO | DGP | - | Discrete Fidelity | - | [Python](https://github.com/luck1226/multisource_deepGaussianProcess) | [PDF](https://arxiv.org/pdf/1903.07320v1.pdf) |
| 5  | Perdikaris et al., 2017, *Proc. R. Soc. A* (cited by 296) | MFBO | DGP | - | Discrete Fidelity | - | [Python](https://github.com/paraklas/NARGP/tree/master) | [PDF](https://www.researchgate.net/profile/Paris-Perdikaris-2/publication/313482464_Nonlinear_information_fusion_algorithms_for_data-efficient_multi-fidelity_modelling/links/58a0ab0baca272046aad5f88/Nonlinear-information-fusion-algorithms-for-data-efficient-multi-fidelity-modelling.pdf) |
| 6  | Requeima et al., 2019, *AISTAS* (cited by 38) | MFBO | DGP | - | Discrete Fidelity | - | [Python](https://github.com/wesselb/gpar) | [PDF](https://arxiv.org/pdf/1802.07182v4.pdf) |
| 7  | Damianou & Lawrence, 2013, *AISTATS* (cited by 1203) | MFBO | DGP | - | Discrete Fidelity | - | [Python](https://github.com/SheffieldML/PyDeepGP) | [PDF](http://proceedings.mlr.press/v31/damianou13a.pdf) |
| 8  | Salimbeni & Deisenroth, 2017, *NeurIPS* (cited by 407) | MFBO | DGP | - | Discrete Fidelity | - | [Python](https://paperswithcode.com/paper/doubly-stochastic-variational-inference-for) | [PDF](https://arxiv.org/pdf/1705.08933v2.pdf) |

---

# 2. Surrogate-assisted EAs for MFO

| #  | Paper | Framework | Model | Fidelity Type | Application | Code | PDF |
|----|---------------------------------------------|------------|------|--------------|--------------|----|----|
| 1  | Wang H, Jin Y, Doherty J., 2017, *IEEE Trans. Evol.* (cited by 2) | Surrogate-assisted EA | - | Multi-fidelity | Generic Test Suite | [Matlab](https://github.com/HandingWang/MFB) | [PDF](https://ieeexplore.ieee.org/document/8054707) |
| 2  | Wang H, Jin Y, Yang C, et al., 2020, *Applied Soft Computing* (cited by 2) | Surrogate-assisted EA | - | Multi-fidelity | Bi-Fidelity Evolutionary Algorithm | [Matlab](https://github.com/HandingWang/TSA-BFEA) | [PDF](https://www.sciencedirect.com/science/article/pii/S1568494620302167) |
| 3  | Kenny A, Ray T, Singh H K, et al., 2023, *EMO’23* | Surrogate-assisted EA | - | Multi-objective Multi-fidelity | - | [Python](http://www.mdolab.net/research_resources.html) | [PDF](https://link.springer.com/chapter/10.1007/978-3-031-27250-9_26) |

---

# 3. Bandit-based MF Algorithm

| #  | Paper | Framework | Model | Fidelity Type | Code | PDF |
|----|---------------------------------------------|------------|------|--------------|----|----|
| 1  | **Jamieson K, Talwalkar A.**, 2016, *PMLR'16* (cited by 519) | Bandit | No | Discrete Fidelity | [R](https://github.com/mlr-org/mlr3hyperband) | [PDF](https://arxiv.org/pdf/1502.07943v1.pdf) |
| 2  | **Li L, Jamieson K, DeSalvo G, et al.**, 2017, *ICLR'17* (cited by 2123) | Bandit | No | Discrete Fidelity | [Python](https://github.com/automl/HpBandSter) | [PDF](https://liamcli.com/assets/pdf/hyperband_iclr.pdf) |
| 3  | **Falkner S, Klein A, Hutter F.**, 2018, *PMLR’18* (cited by 914) | Bandit | TPE | Discrete Fidelity | [Python](https://github.com/automl/HpBandSter) | [PDF](https://arxiv.org/pdf/1807.01774v1.pdf) |
| 4  | **Lindauer M, Eggensperger K, Feurer M, et al.**, 2022, *JMLR* (cited by 914) | Bandit | TPE | Discrete Fidelity | [Python](https://github.com/automl/HpBandSter) | [PDF](https://www.jmlr.org/papers/volume23/21-0888/21-0888.pdf) |
| 5  | **Li L, Jamieson K, Rostamizadeh A, et al.**, 2020, *MLSys20* (cited by 244) | Bandit | No | Discrete Fidelity | [Python](https://paperswithcode.com/paper/massively-parallel-hyperparameter-tuning) | [PDF](https://arxiv.org/pdf/1810.05934v5.pdf) |
| 6  | **Awad N H, Mallik N, Hutter F.**, 2021, *IJCAI'21* (cited by 50) | Bandit | No | Discrete Fidelity | [Python](https://paperswithcode.com/paper/dehb-evolutionary-hyberband-for-scalable) | [PDF](https://arxiv.org/pdf/2105.09821v2.pdf) |
| 7  | **Li Y, Shen Y, Jiang J, et al.**, 2021, *AAAI'21* (cited by 15) | Bandit | Random Forest | Discrete Fidelity | [Python](https://paperswithcode.com/paper/mfes-hb-efficient-hyperband-with-multi) | [PDF](https://arxiv.org/pdf/2012.03011v2.pdf) |
| 8  | **Li Y, Shen Y, Jiang H, et al.**, 2022, *VLDB’22* (cited by 8) | Bandit | Random Forest | Discrete Fidelity | [Python](https://github.com/thomas-young-2013/HyperTune) | [PDF](https://arxiv.org/pdf/2201.06834v1.pdf) |
| 9  | **Bohdal O, Balles L, Ermis B, et al.**, 2022, *arXiv* (cited by 4) | Bandit | No | Discrete Fidelity | [Python](https://paperswithcode.com/paper/pasha-efficient-hpo-with-progressive-resource) | [PDF](https://arxiv.org/pdf/2207.06940v2.pdf) |
| 10 | **Zhu X, Liu Y, Ghysels P, et al.**, 2022, *SIAM Conf. Parallel Processing* (cited by 2) | Bandit | LMC | Discrete Fidelity | [Python](https://github.com/gptune/GPTune) | [PDF](https://crd.lbl.gov/assets/Uploads/GPTuneBand.pdf) |

---

This structured table format ensures clarity and ease of reference. Let me know if you need further refinements! 🚀
