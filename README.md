# MF literature review list

<aside>
💡 This is the notebook for recording MF optimization literature in preparation for the CSUR paper.

</aside>

# 1. Multi-Fidelity Surrogate Model

We provide an overview of various approaches to build a surrogate model for multi-fidelity data, with a focus on their application in MFO.

## 1.1 Single model methods

### 1.1.1 RSM

1. Giunta A A, Balabanov V, Kaufman M, et al. Variable-complexity response surface design of an HSCT configuration[J]. Multidisciplinary Design Optimization, Alexandrov NM and Hussaini MY eds, 1997, cited by 42. 
    
    [Problem ](https://www.notion.so/Problem-8b25a34918624e048a55e148f84b9457?pvs=21)
    
    ▪️ Application: aerodynamic-structural optimization of the High Speed Civil Transport (HSCT) 
    

### 1.1.2 GP

1. Liu B, Koziel S, Zhang Q. A multi-fidelity surrogate-model-assisted evolutionary algorithm for computationally expensive optimization problems[J]. **`*J. Comput. Sci.*`**, 2016, cited by 115.
2. Kandasamy K, Dasarathy G, Oliva J, et al. Multi-fidelity gaussian process bandit optimisation[J]. `*J. Artif. Intell. Res.*`, 2016, cited by 75. 
    
    🗓️ 2016  📄 `*J. Artif. Intell. Res.*`
    
     ▪️ Framework: MFBO ▪️ Model: single model-GP ▪️ Fidelity Management: UCB  ▪️ Discrete Fidelity 
    
    [Code-Matlab](https://github.com/kirthevasank/mf-gp-ucb)
    
    [PDF](https://www.jair.org/index.php/jair/article/view/11288)
    
3. Folch J P, Lee R M, Shafei B, et al. Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization[J]. **`*Comput. Chem. Eng.*`**, 2023, cited by 7.  ****
    
    ▪️ Framework: MFBO ▪️ Model: GP/MTGP ▪️ Fidelity Management: UCB/MES asynchronous batch  ▪️ Discrete Fidelity ▪️ Application: materials for optimal performance in pouch cells.
    

### 1.1.3 RBF

1. Liu B, Koziel S, Zhang Q. A multi-fidelity surrogate-model-assisted evolutionary algorithm for computationally expensive optimization problems[J]. **`*J. Comput. Sci.*`**, 2016, cited by 115.
2. Yi J, Shen Y, Shoemaker C A. A multi-fidelity RBF surrogate-based optimization framework for computationally expensive multi-modal problems with application to capacity planning of manufacturing systems[J]. `*Struct. Multidiscip. Optim.*`, 2020, cited by 20.
3. Kampolis I C, Zymaris A S, Asouti V G, et al. Multilevel optimization strategies based on metamodel-assisted evolutionary algorithms, for computationally expensive problems, `*CEC’07*`. 2007, cited by 37.

## 1.2 Correction-based methods

### 1.2.1 First-order Taylor series

1. Haftka R T. Combining global and local approximations, `*AIAA*`, 1991, cited by 192.
2. Chang K J, Haftka R T, Giles G L, et al. Sensitivity-based scaling for approximating structural response, **`*J. Aircr.*`**, 1993, 30(2): 283-288, cited by 150.
3. Lewis R, Nash S. A multigrid approach to the optimization of systems governed by differential equations, 8th symposium on multidisciplinary analysis and optimization. 2000, cited by 108.

### 1.2.2 Second-order Taylor series

1. Eldred M, Giunta A, Collis S. Second-order corrections for surrogate-based optimization with model hierarchies, 10th AIAA/ISSMO multidisciplinary analysis and optimization conference. 2004, cited by 221.
2. Gano S, Perez V, Renaud J, et al. Multilevel variable fidelity optimization of a morphing unmanned aerial vehicle[C]//45th AIAA/ASME/ASCE/AHS/ASC Structures, Structural Dynamics & Materials Conference. 2004, cited by 41.

## 1.3 Autoregressive-based (AR1) methods

1. Zhang L, Wu Y, Jiang P, et al. A multi-fidelity surrogate modeling approach for incorporating multiple non-hierarchical low-fidelity data[J]. **`*Adv. Eng. Inform.*`**, 2022, cited by 12. 
    
    ▪️ Model: non-hierarchical Co-Kriging modelling ▪️ Fidelity Management: UCB/MES asynchronous batch  ▪️ Discrete Fidelity ▪️ Application: prediction of the maximum Von Mises stress for a cylindrical pressure vessel containing natural gas
    

## 1.4 Multi-task GP (MTGP) methods

1. Folch J P, Lee R M, Shafei B, et al. Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization[J]. **`*Comput. Chem. Eng.*`**, 2023, cited by 7.
    
    ▪️ Framework: MFBO ▪️ Model: GP/MTGP ▪️ Fidelity Management: UCB/MES asynchronous batch  ▪️ Discrete Fidelity ▪️ Application: materials for optimal performance in pouch cells.
    
    [Code-Python](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078)
    
    [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637)
    
2. Mikkola P, Martinelli J, Filstroff L, et al. Multi-Fidelity Bayesian Optimization with Unreliable Information Sources[C]. `*AISTATS’23*`, 2023, cited by 1.
    
    ▪️ Framework: MFBO ▪️ Model: MTGP ▪️ Fidelity Management: MES  ▪️ Continuous Fidelity: learners trees ▪️ Application: XGBoost (diabetes progression)
    
    [Code-Python](https://github.com/aaltopml/rmfbo)
    
    [Mikkola23](https://proceedings.mlr.press/v206/mikkola23a/mikkola23a.pdf)
    
3. Lin Q, Qian J, Cheng Y, et al. A multi-output multi-fidelity Gaussian process model for non-hierarchical low-fidelity data fusion[J]. `*Knowl. Based Syst.*`, 2022, cited by 4.

## 1.5 Nonlinear hierarchical methods

1. Savage T, Basha N, Ehecatl O M, et al. Deep Gaussian Process-based Multi-fidelity Bayesian Optimization for Simulated Chemical Reactors,`*NeurIPS’22*`,2022, cited by 3.
    
    ▪️ Framework: MFBO ▪️ Model: DGP ▪️ Fidelity Management: UCB  ▪️ Discrete Fidelity ▪️ Application: chemical reactor designs
    
    [Code-Python](https://github.com/optimal-pse-lab/pulsed-reactor-optimisation)
    
    [Savage22](https://arxiv.org/pdf/2210.17213.pdf)
    
2. Xu Y, Song X, Zhang C. Hierarchical regression framework for multi-fidelity modeling[J]. `*Knowl. Based Syst.*`, 2021,  cited by 6. 
    
    ▪️ Model: Hierarchical   ▪️ Discrete Fidelity ▪️ Prediction
    
3. **[IMPORTANT]** K. Cutajar, M. Pullin, A. C. Damianou, N. D. Lawrence, and J. Gonzalez, “Deep Gaussian processes for multi-fidelity modeling,” `*arXiv*`, 2019, cited by 94.
    
    ▪️ Model: DGP  ▪️ Discrete Fidelity 
    
    [Code-Python](https://github.com/luck1226/multisource_deepGaussianProcess)
    
    [Cutajar19](https://arxiv.org/pdf/1903.07320v1.pdf)
    
4. **[IMPORTANT]** P. Perdikaris, M. Raissi, A. Damianou, N. D. Lawrence, and G. E. Karniadakis, “Nonlinear information fusion algorithms for data-efficient multi-fidelity modeling,” `*Proc. R. Soc. A: Math. Phys. Eng. Sci.*`, 2017, cited by 296.
    
    ▪️ Model: DGP  ▪️ Discrete Fidelity 
    
    [Code-Python](https://github.com/paraklas/NARGP/tree/master)
    
    [Perdikaris17.pdf](https://www.researchgate.net/profile/Paris-Perdikaris-2/publication/313482464_Nonlinear_information_fusion_algorithms_for_data-efficient_multi-fidelity_modelling/links/58a0ab0baca272046aad5f88/Nonlinear-information-fusion-algorithms-for-data-efficient-multi-fidelity-modelling.pdf)
    
5. **[IMPORTANT]**  J. Requeima, W. Tebbutt, W. Bruinsma, and R. E. Turner, “The Gaussian process autoregressive regression model (GPAR),” `*AISTAS’19*`, pp. 1860–1869, cited by 38.
    
    ▪️ Model: DGP  ▪️ Discrete Fidelity 
    
    [Code-Python](https://github.com/wesselb/gpar)
    
    [Requeima19](https://arxiv.org/pdf/1802.07182v4.pdf)
    
6. **[IMPORTANT]**  A. C. Damianou and N. D. Lawrence, “Deep gaussian processes,”  **`AISTATS’13`**, 2013, cited by 1203.
    
    ▪️ Model: DGP  ▪️ Discrete Fidelity 
    
    [Code-Python](https://github.com/SheffieldML/PyDeepGP)
    
    [Damianou13.pdf](http://proceedings.mlr.press/v31/damianou13a.pdf)
    
7. [**[IMPORTANT]**  H. Salimbeni and M. P. Deisenroth, “Doubly stochastic variational inference for deep gaussian processes,” `*NeurIPS’17*`, 2017, cited by  407.
    
    ▪️ Framework: MFBO ▪️ Model: DGP  ▪️ Discrete Fidelity 
    
    [Code-Python](https://paperswithcode.com/paper/doubly-stochastic-variational-inference-for)
    
    [Salimbeni17](https://arxiv.org/pdf/1705.08933v2.pdf)
    
8. **[IMPORTANT]**  S. Li, W. Xing, R. M. Kirby, and S. Zhe, “Multi-fidelity Bayesian optimization via deep neural networks,” `*NeurIPS’20*`,2020, cited by 33.
    
    ▪️ Framework: MFBO ▪️ Model: DNN  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES
    
    [Code-Python](https://www.notion.soCode-Python)
    
    [Li20](https://arxiv.org/pdf/2007.03117v4.pdf)
    
9. **[IMPORTANT]**  S. Li, R. M. Kirby, and S. Zhe, “Batch multi-fidelity Bayesian optimization with deep auto-regressive networks,” in `*NeurIPS’21*`, 2021, pp. 25 463–25 475, cited by 33.
    
    ▪️ Framework: MFBO ▪️ Model: DNN  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES
    
    [Code-Python](https://github.com/shib0li/BMBO-DARN)
    
    [Li21](https://arxiv.org/pdf/2106.09884v2.pdf)
    
10. **[IMPORTANT]**  Y. Xu, X. Song, and C. Zhang, “Hierarchical regression framework for multi-fidelity modeling,” `*Knowl. Based Syst.*`, 2021, cited by  6.

## 1.6 single GP for continuous fidelity

1. Savage T, Basha N, McDonough J, et al. Multi-Fidelity Data-Driven Design and Analysis of Reactor and Tube Simulations[J]. arXiv preprint `*arXiv*`:2305.00710, 2023, cited by 3. 
    
    ▪️ Fidelity Management: MES  ▪️ Optimization ▪️ Application: chemical reactor designs
    
2. Winter J M, Abaidi R, Kaiser J W J, et al. Multi-fidelity Bayesian optimization to solve the inverse Stefan problem[J].Comput. `*Methods Appl. Mech. Eng.*`, 2023, cited by 1. 
    
    ▪️ Fidelity Management: cfKG acquisition function  ▪️ Optimization ▪️ Application: inverse Stefan problem
    

## 1.7 Space mapping methods

1. **[IMPORTANT]** Bandler, J. W., Biernacki, R. M., Chen, S. H., Grobelny, P. A., and Hemmers, R. H.(1994). Space mapping technique for electromagnetic optimization. IEEE Transactions on Microwave Theory and Techniques, 42(12):2536–2544.cited by 833.
2. **[IMPORTANT]** Bandler, J., Biernacki, R., Chen, S., Hemmers, R., and Madsen, K., “Electromagnetic Optimization Exploiting Aggressive Space Mapping,” IEEE Transactions on Microwave Theory and Techniques, Vol. 43, No. 12, Dec. 1995, pp. 2874–2882.cited by 482. **[aggressive space mapping]**
3. Bandler, J., Biernacki, R., and Chen, S., “Fully Automated Space Mapping Optimization of 3D Structures,” Proceedings of the IEEE MTT-S International Microwave Symposium, Inst. of Electrical and Electronics Engineers, Piscataway, NJ, June 1996, pp. 753–756.cited by 57.
4. **[IMPORTANT]** Bakr, M. H., Bandler, J. W., Biernacki, R. M., Chen, S. H., and Madsen, K. (1998). A trust region aggressive space mapping algorithm for em optimization. IEEE Transactions on Microwave Theory and Techniques, 46(12):2412–2425. cited by 177.**[trust regions]**
5. Bakr M H, Bandler J W, Georgieva N, et al. A hybrid aggressive space-mapping algorithm for EM optimization[J]. IEEE Transactions on Microwave Theory and Techniques, 1999, 47(12): 2440-2449..cited by 134.**[trust regions]**
6. **[IMPORTANT-SANDIA REPORT]** Castro, J. P. J., Gray, G. A., Hough, P. D., and Giunta, A. A., “Developing a computationally efficient dynamic multilevel hybrid optimization scheme using multifidelity model interactions,” Tech. rep., SAND2005-7498, Sandia National Laboratories. Albuquerque, NM, 2005.cited by 17.
7. Bakr, M. H., Bandler, J. W., Ismail, M. A., Rayas-Sánchez, J. E., and Zhang, Q. J.(2000). Neural space mapping em optimization of microwave structures. In IEEE MTT-S International Microwave Symposium Digest, volume 2, pages 879–882. cited by 26.**[artificial neural networks]**
8. **[IMPORTANT]** Robinson, T., Eldred, M., Willcox, K., and Haimes, R., “Surrogate-based optimization using multifidelity models with variable parameterization and corrected space mapping,” AIAA Journal, Vol. 46, No. 11, 2008, pp. 2814–2822.cited by 278. 
9. Jonsson, I. M., Leifsson, L., Koziel, S., Tesfahunegn, Y. A., and Bekasiewicz, A., “Shape Optimization of Trawl-doors Using Variable-fidelity Models and Space Mapping,” Procedia Computer Science, Vol. 51, 2015, pp. 905–913. cited by 27. 
10. Ren, J., Leifsson, L., Koziel, S., and Tesfahunegn, Y., “Multi-Fidelity Aerodynamic Shape Optimization Using Manifold Mapping,” 57th AIAA/ASCE/AHS/ASC Structures, Structural Dynamics, and Materials Conference, 2016. cited by 15. **[Manifold Mapping]**
11. Koziel, S., Tesfahunegn, Y., Amrit, A., and Leifsson, L., “Rapid Multi-Objective Aerodynamic Design Using Co-Kriging and Space Mapping,” 57th AIAA/ASCE/AHS/ASC Structures, Structural Dynamics, and Materials Conference, 2016. cited by 20. [not important]
12. Madsen, K., and Søndergaard, J., “Convergence of Hybrid Space Mapping Algorithms,” Optimization and Engineering, Vol. 5, No. 2, June 2004, pp. 145–156. cited by 29.
13. Bandler, J. W., Cheng, Q. S., Nikolova, N. K., and Ismail, M. A. (2004b). Implicit space mapping optimization exploiting preassigned parameters. IEEE Transactions on Microwave Theory and Techniques, 52(1):378–385.**[implicit space mapping]**
14. Zhang, L., Xu, J., Yagoub, M. C., Ding, R., and Zhang, Q.-J. (2005). Efficient analytical formulation and sensitivity analysis of neuro-space mapping for nonlinear microwave device modeling. IEEE transactions on microwave theory and techniques, 53(9):2752–2767.**[neural-based space mapping]**
15.  Zhang, L., Zhang, Q.-J., and Wood, J. (2008). Statistical neuro-space mapping technique for large-signal modeling of nonlinear devices. IEEE Transactions on Microwave Theory and Techniques, 56(11):2453–2467.**[neural-based space mapping]**
16. 141. Rayas-Sánchez, J. E., Lara-Rojo, F., and Martínez-Guerrero, E. (2005). A linear inverse space-mapping (lism) algorithm to design linear and nonlinear rf andmicrowave circuits. IEEE transactions on microwave theory and techniques, 53(3):960–968 **[inverse problems]**
17. Koziel, S., Meng, J., Bandler, J. W., Bakr, M. H., and Cheng, Q. S. (2009). Accelerated microwave design optimization with tuning space mapping. IEEE Transactions on Microwave Theory and Techniques, 57(2):383–394.**[tuning space mapping]**

---

# 2. Bayesian Optimization for MFO

## 2.1 Single model-based MFBO

## 2.2 Correction-based MFBO

1. Folch J P, Lee R M, Shafei B, et al. Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization[J]. **`*Comput. Chem. Eng.*`**, 2023, cited by 7.
    
    ▪️ Framework: MFBO ▪️ Model: GP/MTGP ▪️ Fidelity Management: UCB/MES asynchronous batch  ▪️ Discrete Fidelity ▪️ Application: materials for optimal performance in pouch cells.
    
    [Code-Python](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078)
    
    [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637)
    
2. Zhang S, Liang P, Pang Y, et al. Multi-fidelity surrogate model ensemble based on feasible intervals[J]. Structural and Multidisciplinary Optimization, 2022, 65(8): 212, cited by 3.
    
    ▪️ Model: kriging ▪️ Discrete Fidelity ▪️ Prediction ▪️ Application: electrode materials for optimal performance in pouch cells
    

## 2.3 AR1-based MFBO

1. Di Fiore F, Mainini L. Non-myopic multifidelity bayesian optimization[J]. arXiv preprint arXiv:2207.06325, 2022, cited by 3.
    
    ▪️ Discrete Fidelity 
    

## 2.4 MTGP-based MFBO

1. Wistuba M, Kadra A, Grabocka J. Supervising the multi-fidelity race of hyperparameter configurations[J]. `*NeurIPS’22*`, 2022, cited by 3. 
    
    ▪️ Framework: MFBO ▪️ Model: deep kernel+GP ▪️ Fidelity Management: gradually increase.
    
    [Code-Python](https://github.com/releaunifreiburg/DyHPO)
    
    [Wistuba22](https://arxiv.org/pdf/2202.09774v2.pdf)
    
2. Klein A, Falkner S, Bartels S, et al. Fast bayesian optimization of machine learning hyperparameters on large datasets[C]. `*AISTATS’17*`, 2017, cited by 592.
    
    ▪️ Framework: MFBO ▪️ Model: GP  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES
    
    [Code-Python](https://github.com/automl/RoBO)
    
    [Klein17](https://arxiv.org/pdf/1605.07079v2.pdf)
    
3. Kandasamy K, Dasarathy G, Schneider J, et al. Multi-fidelity bayesian optimisation with continuous approximations. `*ICML’17*`, 2017, cited by 201. 
    
    ▪️ Framework: MFBO ▪️ Model: GP  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES. Discrete/continuous Fidelity
    
    [Code-Python](https://github.com/cclauss/dragonfly/tree/16071860ff2a182cf8854f11c1a7006bcae58267)
    
    [Kandasamy17](https://arxiv.org/pdf/1703.06240v1.pdf)
    
4. Wu J, Toscano-Palmerin S, Frazier P I, et al. Practical multi-fidelity bayesian optimization for hyperparameter tuning[C]. `*UAI’20*`, 2020, cited by 113.
    
    ▪️ Framework: MFBO ▪️ Model: GP  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES. Discrete/continuous Fidelity
    
    [Wu20](https://arxiv.org/pdf/1903.04703v1.pdf)
    
5. Folch J P, Lee R M, Shafei B, et al. Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization[J]. **`*Comput. Chem. Eng.*`**, 2023, cited by 7.
    
    ▪️ Framework: MFBO ▪️ Model: GP/MTGP ▪️ Fidelity Management: UCB/MES asynchronous batch  ▪️ Discrete Fidelity ▪️ Application: materials for optimal performance in pouch cells.
    
    [Code-Python](https://www.notion.so/colalab/MF-literature-review-list-bbc9c0aacb7b46109f1af12bc69f85aa?pvs=4#198c2fbcd85c45f6b4eeb78bdadbe078)
    
    [PDF](https://www.sciencedirect.com/science/article/pii/S0098135423000637)
    
6. Takeno S, Fukuoka H, Tsukada Y, et al. A generalized framework of multifidelity max-value entropy search through joint entropy[J]. `*Neural Comput.*`, 2022, 34(10): 2145-2203, cited by 4. 
    
    ▪️ Framework: MFBO ▪️ Model: MTGP  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES ▪️ Application: SVM, Material data
    

## 2.5 Nonlinear hierarchical-based MFBO

1. **[IMPORTANT]** Li S, Xing W, Kirby R, et al. Multi-fidelity Bayesian optimization via deep neural networks[J]. `*NeurIPS’20*`, 2020, cited by 33. 
    
    ▪️ Framework: MFBO ▪️ Model: DNN  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES
    
    [Code-Python](https://www.notion.soCode-Python)
    
    [Li20](https://arxiv.org/pdf/2007.03117v4.pdf)
    
2. **[IMPORTANT]**  S. Li, R. M. Kirby, and S. Zhe, “Batch multi-fidelity Bayesian optimization with deep auto-regressive networks,” in NeurIPS’21: Proc. of the Annual Conference on Neural Information Processing Systems 2021, 2021, pp. 25 463–25 475, cited by 33
    
    ▪️ Framework: MFBO ▪️ Model: DNN  ▪️ Discrete Fidelity ▪️ Fidelity Management: MES
    
    [Code-Python](https://github.com/shib0li/BMBO-DARN)
    
    [Li21](https://arxiv.org/pdf/2106.09884v2.pdf)
    
3. Savage T, Basha N, Ehecatl O M, et al. Deep Gaussian Process-based Multi-fidelity Bayesian Optimization for Simulated Chemical Reactors,`*NeurIPS’22*`,2022, cited by 3.
    
    ▪️ Framework: MFBO ▪️ Model: DGP ▪️ Fidelity Management: UCB  ▪️ Discrete Fidelity ▪️ Application: chemical reactor designs
    
    [Code-Python](https://github.com/optimal-pse-lab/pulsed-reactor-optimisation)
    
    [Savage22](https://arxiv.org/pdf/2210.17213.pdf)
    

---

# 3. Surrogate-assisted EAs for MFO

1. Yi J, Shen Y, Shoemaker C A. A multi-fidelity RBF surrogate-based optimization framework for computationally expensive multi-modal problems with application to capacity planning of manufacturing systems[J]. `*Struct. Multidiscip. Optim.*`, 2020, cited by 20. **Optimization,** .
    
    ▪️ Optimization ▪️ Application: capacity planning for manufacturing systems
    
2. Kenny A, Ray T, Singh H K. An iterative two-stage multi-fidelity optimization algorithm for computationally expensive problems[J]. `*IEEE Trans. Evol.*`, 2022, cited by 2. 
3. Kenny A, Ray T, Singh H K, et al. A Test Suite for Multi-objective Multi-fidelity Optimization, `*EMO’23*`, 2023.
    
    [Code-Python](http://www.mdolab.net/research_resources.html)
    
    [Kenny23.pdf](https://link.springer.com/chapter/10.1007/978-3-031-27250-9_26)
    

---

# 4. Bandit-based MF Algorithm

---

> The bandit-based MF algorithms mainly focus on improving the efficiency of the Hyperband. Use the model(TPE/ensemble) to help the sampling.
> 
1. Karnin Z, Koren T, Somekh O. “Almost optimal exploration in multi-armed bandits”, International Conference on Machine Learning. `*PMLR'13*`, 2013, cited by 437.
2. **[IMPORTANT]** Jamieson K, Talwalkar A. “Non-stochastic best arm identification and hyperparameter optimization”, Artificial intelligence and statistics. `*PMLR'16*`, 2016, cited by 519.
    
    ▪️ Framework: Bandit ▪️ Model: No  ▪️ Discrete Fidelity
    
    [Code-R](https://github.com/mlr-org/mlr3hyperband)
    
    [Jamieson16](https://arxiv.org/pdf/1502.07943v1.pdf)
    
3. **[IMPORTANT]** Li L, Jamieson K, DeSalvo G, et al. “Hyperband: Bandit-based configuration evaluation for hyperparameter optimization”, `*ICLR'17*`, 2017, cited by 2123.
    
    ▪️ Framework: Bandit ▪️ Model: No  ▪️ Discrete Fidelity
    
    [Code-Python](https://github.com/automl/HpBandSter)
    
    [Li17](https://liamcli.com/assets/pdf/hyperband_iclr.pdf)
    
4. Bertrand H, Ardon R, Perrot M, et al. “Hyperparameter optimization of deep neural networks: Combining hyperband with Bayesian model selection”, `*CAp'17*`, 2017, cited by 33.
5. Wang J, Xu J, Wang X. “Combination of hyperband and Bayesian optimization for hyperparameter optimization in deep learning”,`*arXiv*`, 2018, cited by 67.
6. **[IMPORTANT]** Falkner S, Klein A, Hutter F. “BOHB: Robust and efficient hyperparameter optimization at scale”,  `*PMLR’18`,* 2018, cited by 914.
    
    ▪️ Framework: Bandit ▪️ Model: TPE ▪️ Discrete Fidelity
    
    [Code-Python](https://github.com/automl/HpBandSter)
    
    [Falkner18](https://arxiv.org/pdf/1807.01774v1.pdf)
    
7. **[IMPORTANT]** Li L, Jamieson K, Rostamizadeh A, et al. “A system for massively parallel hyperparameter tuning”, `*MLSys20*`, 2020, cited by 244.
    
    ▪️ Framework: Bandit ▪️ Model: No ▪️ Discrete Fidelity
    
    [Code-Python](https://paperswithcode.com/paper/massively-parallel-hyperparameter-tuning)
    
    [Li20](https://arxiv.org/pdf/1810.05934v5.pdf)
    
8. **[IMPORTANT]** Awad, Noor H., Neeratyoy Mallik and Frank Hutter. “DEHB: Evolutionary Hyberband for Scalable, Robust and Efficient Hyperparameter Optimization”, `*IJCAI'21*`, 2021, cited by 50.
    
    ▪️ Framework: Bandit ▪️ Model: No ▪️ Discrete Fidelity
    
    [Code-Python](https://paperswithcode.com/paper/dehb-evolutionary-hyberband-for-scalable)
    
    [Awad21](https://arxiv.org/pdf/2105.09821v2.pdf)
    
9. **[IMPORTANT]** Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15.
    
    ▪️ Framework: Bandit ▪️ Model: Random Forest ▪️ Discrete Fidelity
    
    [Code-Python](https://paperswithcode.com/paper/mfes-hb-efficient-hyperband-with-multi)
    
    [Li21](https://arxiv.org/pdf/2012.03011v2.pdf)
    
10. **[IMPORTANT]** Li Y, Shen Y, Jiang H, et al. “Hyper-tune: towards efficient hyper-parameter tuning at scale”,  `*VLDB’22*`, 2022, cited by 8.
    
    ▪️ Framework: Bandit ▪️ Model: Random Forest  ▪️ Discrete Fidelity
    
    [Code-Python](https://github.com/thomas-young-2013/HyperTune)
    
    [Li22](https://arxiv.org/pdf/2201.06834v1.pdf)
    
11. **[IMPORTANT]** Bohdal O, Balles L, Ermis B, et al. “PASHA: Efficient HPO with Progressive Resource Allocation”, `*arXiv*`, 2022, cited by 4.
    
    ▪️ Framework: Bandit ▪️ Model: No  ▪️ Discrete Fidelity
    
    [Code-Python](https://paperswithcode.com/paper/pasha-efficient-hpo-with-progressive-resource)
    
    [Bohdal22](https://arxiv.org/pdf/2207.06940v2.pdf)
    
12. Zhu X, Liu Y, Ghysels P, et al. GPTuneBand: Multi-task and Multi-fidelity Autotuning for Large-scale High Performance Computing Applications[C]//Proceedings of the 2022 SIAM Conference on Parallel Processing for Scientific Computing. Society for Industrial and Applied Mathematics, 2022: 1-13, cited by 2.
    
    ▪️ Framework: Bandit ▪️ Model: LMC ▪️ Discrete Fidelity
    
    [Code-Python](https://github.com/gptune/GPTune)
    
    [Zhu22](https://crd.lbl.gov/assets/Uploads/GPTuneBand.pdf)
    

---

# 5. Fidelity Management Strategies

## 5.1 Fixed methods

## 5.2 Adaptive methods

---

# 6. Benchmark Problems in MFO

## 6.1 Synthetic problems

1. Kenny A, Ray T, Singh H K, et al. A Test Suite for Multi-objective Multi-fidelity Optimization, `*EMO’23*`, 2023.
2. Andrés-Thió N, Muñoz M A, Smith-Miles K. Bifidelity Surrogate Modelling: Showcasing the Need for New Test Instances[J]. INFORMS Journal on Computing, 2022, 34(6): 3007-3022.

## 6.2 NAS Benchmark

1. Liu H, Simonyan K, Yang Y. DARTS: Differentiable Architecture Search, `*ICML’18*`, 2018, cited by 3813.
2. Ying C, Klein A, Christiansen E, et al. Nas-bench-101: Towards reproducible neural architecture search, `*ICML’19*`, 2019, cited by 504.
3. Dong X, Yang Y. NAS-Bench-201: Extending the Scope of Reproducible Neural Architecture Search, `*ICML’19*`, 2019, cited by 530.
4. Wang Z, Dahl G E, Swersky K, et al. Pre-trained Gaussian processes for Bayesian optimization, `*arXiv*`, 2021, cited by 9. **xformer**

---

# 7. Application in MF Optimization

## 7.1 HPO (ML model/task/fidelity setting/MF model/optimization)

### 7.1.1 CNN

1. Bohdal O, Balles L, Ermis B, et al. “PASHA: Efficient HPO with Progressive Resource Allocation”, `*arXiv*`, 2022, cited by 4.  **Task**: NASBench201 (CIFAR-10, CIFAR-100,ImageNet16-120); ResNet50( ImageNet). **Fidelity type**: epoch. **Method**: improved Hyperband.
2. Li Y, Shen Y, Jiang H, et al. “Hyper-tune: towards efficient hyper-parameter tuning at scale”,  `*VLDB’22*`, 2022, cited by 8. **Task**: NASBench201 (CIFAR-10-Valid, CIFAR-100,ImageNet16-120); ResNet( CIFAR-10). **Fidelity type**: epoch. **Method**: improved Hyperband.
3. Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15.**Task**: ResNet50( CIFAR-10). **Fidelity type**: epoch. **Method**: improved Hyperband.
4. Awad, Noor H., Neeratyoy Mallik and Frank Hutter. “DEHB: Evolutionary Hyberband for Scalable, Robust and Efficient Hyperparameter Optimization”, `*IJCAI'21*`, 2021, cited by 50.**Task**: NAS-Bench-101 (CIFAR-10); NASBench-1shot1(CIFAR-10); NASBench201 (CIFAR-10, CIFAR-100,ImageNet16-120); ResNet50( ImageNet). **Fidelity type**: epoch. **Method**: improved Hyperband.
5. Li L, Jamieson K, Rostamizadeh A, et al. “A system for massively parallel hyperparameter tuning”, `*MLSys20*`, 2020, cited by 244. **Task**: NAS-Bench-Darts (CIFAR-10); small CNN (CIFAR-10). **Fidelity type**: epoch. **Method**: improved Hyperband.
6. Falkner S, Klein A, Hutter F. “BOHB: Robust and efficient hyperparameter optimization at scale”,  `*PMLR’18`,* 2018, cited by 914.**Task**: medium-sized small CNN (CIFAR-10). **Fidelity type**: epoch. **Method**: improved Hyperband.
7. Wang J, Xu J, Wang X. “Combination of hyperband and Bayesian optimization for hyperparameter optimization in deep learning”,`*arXiv`* , 2018, cited by 67.**Task**: LeNet (MNIST); Alexnet(Cifar10, MRBI, and SVHN). **Fidelity type**: number of training images. **Method**: BO+ Hyperband.
8. Bertrand H, Ardon R, Perrot M, et al. “Hyperparameter optimization of deep neural networks: Combining hyperband with Bayesian model selection”, `*CAp'17*`, 2017, cited by 33.**Task**: CNN (MNIST). **Fidelity type**: epoch. **Method**: BO+ Hyperband.
9. Li L, Jamieson K, DeSalvo G, et al. “Hyperband: Bandit-based configuration evaluation for hyperparameter optimization”, `*ICLR'17*`, 2017, cited by 2123.**Task**: CNN (Cifar10, rotated MNIST, and SVHN). **Fidelity type**: epoch. **Method**: Hyperband.
10. Wistuba M, Kadra A, Grabocka J. Supervising the multi-fidelity race of hyperparameter configurations[J]. `*NeurIPS’22*`, 2022, cited by 3.**Task**: NASBench201 (CIFAR-10, CIFAR-100,ImageNet16-120); . **Fidelity type**: epoch. **Method**: deep kernel+GP. **Fidelity management**: gradually increase.
11. Klein A, Falkner S, Bartels S, et al. Fast bayesian optimization of machine learning hyperparameters on large datasets[C]//Artificial intelligence and statistics. `*PMLR’17*`, 2017, cited by 592. **Task**: CNN with three convolutional layers(CIFAR-10 and SVHN), Resnet(CIFAR-10) . **Fidelity type**: datasize. **Method**: GP. **Fidelity Management**: MES. **Discrete Fidelity.**
12. Wu J, Toscano-Palmerin S, Frazier P I, et al. Practical multi-fidelity bayesian optimization for hyperparameter tuning[C]//Uncertainty in Artificial Intelligence. `*PMLR’20*`, 2020, cited by 113. **Task**: CNN with three convolutional layers(CIFAR-10 and SVHN). **Fidelity type**: data size and epoch. **Method**: MTGP. **Fidelity Management**: MES. **Discrete/cont Fidelity.**
13. Yang S, Tian Y, Xiang X, et al. Accelerating Evolutionary Neural Architecture Search via Multifidelity Evaluation[J]. **`*IEEE Trans.** **Cogn.** **Dev**.*`, 2022, 14(4): 1778-1792, cited by 9. **Task**: NAS(CIFAR-10 , CIFAR-100,ImageNet16-120). **Fidelity type**: epoch and epoch. **Method**: . **Fidelity Management**: gradually increase fidelity. **cont Fidelity.**

### 7.1.2 NLP

1. Bohdal O, Balles L, Ermis B, et al. “PASHA: Efficient HPO with Progressive Resource Allocation”, `*arXiv*`, 2022, cited by 4. **Task**: xformer WMT15 German-English. **Fidelity type**: epoch. **Method**: improved Hyperband.
2. Li Y, Shen Y, Jiang H, et al. “Hyper-tune: towards efficient hyper-parameter tuning at scale”,  `*VLDB’22*`, 2022, cited by 8. **Task**: 3-layer LSTM(Penn Treebank). **Fidelity type**: epoch. **Method**: improved Hyperband.
3. Li L, Jamieson K, Rostamizadeh A, et al. “A system for massively parallel hyperparameter tuning”, `*MLSys20*`, 2020, cited by 244. **Task**: NAS-LSTM(Penn Treebank). **Fidelity type**: epoch. **Method**: improved Hyperband.
4. Wistuba M, Kadra A, Grabocka J. Supervising the multi-fidelity race of hyperparameter configurations[J]. `*NeurIPS’22*`, 2022, cited by 3.**Task**: TaskSet (NLP tabular tasks). **Fidelity type**: epoch. **Method**: deep kernel+GP. **Fidelity management**: gradually increase.

### 7.1.3 MLP

1. Bohdal O, Balles L, Ermis B, et al. “PASHA: Efficient HPO with Progressive Resource Allocation”, `*arXiv*`, 2022, cited by 4.  **Task**: LCBench MLP (openml-cc18). **Fidelity type**: epoch. **Method**: improved Hyperband.
2. Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15.**Task**:  FCNet(MNIST). **Fidelity type**: epoch. **Method**: improved Hyperband.
3. Awad, Noor H., Neeratyoy Mallik and Frank Hutter. “DEHB: Evolutionary Hyberband for Scalable, Robust and Efficient Hyperparameter Optimization”, `*IJCAI'21*`, 2021, cited by 50.**Task**: NAS-HPO-Bench 2-layer feed-forward network( Protein Structure, Slice Localization, Naval Propulsion and Parkinsons Telemonitoring); FNN(Adult, Letter, Higgs, MNIST, Optdigits, Poker). **Fidelity type**: epoch. **Method**: improved Hyperband.
4. Falkner S, Klein A, Hutter F. “BOHB: Robust and efficient hyperparameter optimization at scale”,  `*PMLR’18`,* 2018, cited by 914.**Task**: FNN(Adult, Letter, Higgs, MNIST, Optdigits, Poker). **Fidelity type**: epoch. **Method**: improved Hyperband.
5. Wistuba M, Kadra A, Grabocka J. Supervising the multi-fidelity race of hyperparameter configurations[J]. `*NeurIPS’22*`, 2022, cited by 3.**Task**: LCBench MLP (openml-cc18). **Fidelity type**: epoch. **Method**: deep kernel+GP. **Fidelity management**: gradually increase.
6. Wu J, Toscano-Palmerin S, Frazier P I, et al. Practical multi-fidelity bayesian optimization for hyperparameter tuning[C]//Uncertainty in Artificial Intelligence. `*PMLR’20*`, 2020, cited by 113. **Task**: FNN (MNIST). **Method**: MTGP. **Fidelity Management**: MES. **Discrete/cont Fidelity.**

### 7.1.4 XGB

1. Li Y, Shen Y, Jiang H, et al. “Hyper-tune: towards efficient hyper-parameter tuning at scale”,  `*VLDB’22*`, 2022, cited by 8. **Task**: XGBoost (Pokerhand, Covertype, Hepmass, and Higgs). **Fidelity type**: data size. **Method**: improved Hyperband.
2. Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15. **Task**: XGBoost (Covertype). **Fidelity type**: data size. **Method**: improved Hyperband.
3. Mikkola P, Martinelli J, Filstroff L, et al. Multi-Fidelity Bayesian Optimization with Unreliable Information Sources[C]//International Conference on Artificial Intelligence and Statistics. `*PMLR’23*`, 2023, cited by 1.**Task**: XGBoost (diabetes progression). **Fidelity type**: learners trees. **Method**: MTGP.

### 7.1.5 SVM

1. Li L, Jamieson K, Rostamizadeh A, et al. “A system for massively parallel hyperparameter tuning”, `*MLSys20*`, 2020, cited by 244. **Task**: SVM( ). **Fidelity type**:  . **Method**: improved Hyperband.
2. Falkner S, Klein A, Hutter F. “BOHB: Robust and efficient hyperparameter optimization at scale”,  `*PMLR’18`,* 2018, cited by 914.**Task**: MNIST. **Fidelity type**: datasize. **Method**: improved Hyperband.
3. Klein A, Falkner S, Bartels S, et al. Fast bayesian optimization of machine learning hyperparameters on large datasets[C]//Artificial intelligence and statistics. `*PMLR’17*`, 2017, cited by 592. **Task**: MNIST. **Fidelity type**: datasize. **Method**: GP. **Fidelity Management**: MES. **Discrete Fidelity.**
4. Kandasamy K, Dasarathy G, Schneider J, et al. Multi-fidelity bayesian optimisation with continuous approximations[C]// `*PMLR’17*`, 2017, cited by 201. **Task**: 20 news groups dataset in a text classification task. **Fidelity type**: dataset size and the number of training iterations. **Method**: GP. **Fidelity Management**: MES. **Discrete/cont Fidelity.**

### 7.1.6 BNN

1. Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15. **Task**: regression datasets ( Boston Housing and Protein Structure). **Fidelity type**: MCMC steps. **Method**: improved Hyperband.
2. Falkner S, Klein A, Hutter F. “BOHB: Robust and efficient hyperparameter optimization at scale”,  `*PMLR’18`,* 2018, cited by 914.**Task**: regression datasets ( Boston Housing and Protein Structure). **Fidelity type**: MCMC steps. **Method**: improved Hyperband.

### 7.1.7 RL

1. Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15. **Task**: Cartpole benchmark. **Fidelity type**: Trial number. **Method**: improved Hyperband.
2. Falkner S, Klein A, Hutter F. “BOHB: Robust and efficient hyperparameter optimization at scale”,  `*PMLR’18`,* 2018, cited by 914.**Task**: Cartpole benchmark. **Fidelity type**: Trial number. **Method**: improved Hyperband.

### 7.1.8 Automl

1. Li Y, Shen Y, Jiang J, et al. “MFES-HB: Efficient hyperband with multi-fidelity quality measurements”, `*AAAI'21*`, 2021, cited by 15.**Task**: automl (MNIST, Letter, Higgs, Electricity, Kropt, Mv, Poker, Fried, A9a, 2dplanes,). **Fidelity type**: data size. **Method**: improved Hyperband.
2. Li L, Jamieson K, DeSalvo G, et al. “Hyperband: Bandit-based configuration evaluation for hyperparameter optimization”, `*ICLR'17*`, 2017, cited by 2123.**Task**: automate preprocessing and model selection (117 data sets in openml). **Fidelity type**: data size. **Method**: Hyperband.

### 7.1.9 Other classifiers

1. Li L, Jamieson K, DeSalvo G, et al. “Hyperband: Bandit-based configuration evaluation for hyperparameter optimization”, `*ICLR'17*`, 2017, cited by 2123.**Task**: multi-class regularized least squares classification model (CIFAR-10). **Fidelity type**: data size. random feature kernel approximation classifier (CIFAR-10). **Fidelity type**: feature numbers.**Method**: Hyperband.

### 7.1.10 PINN

1. Penwarden M, Zhe S, Narayan A, et al. Multifidelity modeling for physics-informed neural networks (pinns)[J]. Journal of Computational Physics, 2022, 451: 110844. cited by 24. Fidelity: width, depth, and optimization criteria.
    
    [NN](https://www.notion.so/NN-9a9a95664aa241a39ba0d2bf1fd54b6d?pvs=21)
    
2. Lei J, Liu Q, Wang X. Physics-informed multi-fidelity learning-driven imaging method for electrical capacitance tomography[J]. Engineering Applications of Artificial Intelligence, 2022, 116: 105467.cited by 5.image model：Reconstructing high-accuracy tomograms.

## 7.2 Engineering

### 7.2.1 aircraft optimization

**Fidelity setting**

**Dimensionality**

1. Rajnarayan D, Haas A, Kroo I. A multifidelity gradient-free optimization method and application to aerodynamic design[C]//12th AIAA/ISSMO multidisciplinary analysis and optimization conference. 2008: 6020, cited by 59. **Method**:Correction/GP. **Fidelity Management**:,**Discrete Fidelity:**3D panel method/Area-rule**. Optimization, application**:Axisymmetric Bodies With Low Wave Drag.
2. Toal D J J, Keane A J, Benito D, et al. Multifidelity multidisciplinary whole-engine thermomechanical design optimization[J]. `Journal of Propulsion and Power`, 2014, 30(6): 1654-1666, cited by 43. **Method**:Co-Kriging. **Fidelity Management**:,**Discrete Fidelity:**2D transient thermo-mechanical simulations or 3D mechanical simulations**. Optimization, application**:engine.
3. March A, Willcox K. Constrained multifidelity optimization using model calibration[J]. Structural and Multidisciplinary Optimization, 2012, 46: 93-109, cited by 71. **Method**:Correction,trust region. **Fidelity Management**:No,**Discrete Fidelity:** Cart3D/Linearized panel**. Optimization, application**:supersonic airfoil design.
4. Tao S, Apley D W, Chen W, et al. Input mapping for model calibration with application to wing aerodynamics[J]. AIAA journal, 2019, 57(7): 2734-2745, cited by 24. **Method**:Correction. **Fidelity Management**:No,**Discrete Fidelity:** thin-surface vortex lattice method (VLM) model and a thick-surface vortex ring method (VRM) model**. Optimization, application**:Wing.
5. Lee D, Van Nguyen N, Tyan M, et al. Enhanced multi-fidelity model for flight simulation using global exploration and the Kriging method[J]. Proceedings of the Institution of Mechanical Engineers, Part G: Journal of Aerospace Engineering, 2017, 231(4): 606-620, cited by 8. **Method**:Correction,Kriging. **Fidelity Management**:No,**Discrete Fidelity: AVL, AADL-3D. Optimization, application**:Wing.

**Solver**

1. Ariyarit A, Kanazaki M. Multi-fidelity multi-objective efficient global optimization applied to airfoil design problems[J]. Applied Sciences, 2017, 7(12): 1318, cited by 23. **Method**:Correction. **Fidelity Management**:No,**Discrete Fidelity:** Reynolds-averaged Navier–Stokes (RANS) solver, XFOIL**. Optimization, application**:Airfoil.
2. Nguyen N V, Tyan M, Lee J W. A modified variable complexity modeling for efficient multidisciplinary aircraft conceptual design[J]. Optimization and Engineering, 2015, 16: 483-505, cited by 30. **Method**:Correction. **Fidelity Management**:No,**Discrete Fidelity:** aircraft design synthesis program (ADSP),in-house code AADL3D**. Optimization, application**:regional jet aircraft (RJA) conceptual design,wing.
    
    [Fidelity](https://www.notion.so/Fidelity-4b58f07e8ce340a89ba859499dd4cb5e?pvs=21)
    
3. Gano S, Perez V, Renaud J, et al. Multilevel variable fidelity optimization of a morphing unmanned aerial vehicle[C]//45th AIAA/ASME/ASCE/AHS/ASC Structures, Structural Dynamics & Materials Conference. 2004, cited by 41. **Method**:Correction. **Fidelity Management**:No,**Discrete Fidelity:FUN2D, a full Navier-Stokes coded/ vortex panel method,. Optimization, application**:Buckle Wing. 
    
    [Fidelity](https://www.notion.so/Fidelity-6584c661a70646a9a2ac8f255f85c212?pvs=21)
    
4. Tancred J, Rumpfkeil M P. Aerodynamic response quantification of complex hypersonic configurations using variable fidelity surrogate modeling[C]//53rd AIAA aerospace sciences meeting. 2015, cited by 4. **Method**:Correction. **Fidelity Management**:No,**Discrete Fidelity:** Cart3D/Modified Newtonian Method,**. Optimization, application**:hypersonic nvehicle design.
    
    [](https://www.notion.so/7cfbc6acf83747e69c66809c7bbdf51c?pvs=21)
    

**simplified governing equations**

1. Huang L, Gao Z, Zhang D. Research on multi-fidelity aerodynamic optimization methods[J]. Chinese Journal of Aeronautics, 2013, 26(2): 279-286, cited by 71. **Method**:CO-Kriging. **Fidelity Management**:No,**Discrete Fidelity: Reynolds-averaged Navier–Stokes (RANS) equations,**full potential coupled with boundary layer (BLFP) numerical method**. Optimization, application**:Wing.

**Coarser computational description**

1. Alexandrov, N. M., Lewis, R. M., Gumbert, C. R., Green, L. L., and Newman, P. A., “Optimization with Variable-Fidelity Models Applied to Wing Design,” 38th Aerospace Science Meeting and Exibit, Reno, NV, Jan. 2000. doi:10.2514/6.2000-841.
2. Leifsson, L., and Koziel, S., “Multi-Fidelity Design Optimization of Transonic Airfoils Using Shape-Preserving Response Prediction,” Procedia Computer Science, Vol. 1, No. 1, 2010, pp. 1311–1320. doi:10.1016/j.jocs.2010.03.007.

**Relaxed convergence criteria**

1. Leifsson, L., and Koziel, S., “Multi-Fidelity Design Optimization of Transonic Airfoils Using Shape-Preserving Response Prediction,” `*Procedia Computer Science*`, Vol. 1, No. 1, 2010, cited by 

**simulation and experiments**

1. Tao J, Sun G. Application of deep learning based multi-fidelity surrogate model to robust aerodynamic design optimization[J]. Aerospace Science and Technology, 2019, 92: 722-737, cited by 114. **Method**:Correction,DBN. **Fidelity Management**:No,**Discrete Fidelity: RANS code, real experiment. Optimization, application**:RAE 2822 airfoil model and the DLR-F6 wing-body model.
2. Pellegrini R, Leotardi C, Iemma U, et al. A multi-fidelity adaptive sampling method for metamodel-based uncertainty quantification of computer simulations[C]//Proceedings of the VII European congress on computational methods in applied sciences and engineering, ECCOMAS. 2016, cited by 7. **Method**:Correction,. **Fidelity Management**:No,**Discrete Fidelity: Hydrodynamic Solver, Fluid-Structure Interaction Solver. Optimization, application**:3D NACA 0009 stainless steel hydrofoil.
3. Goldfeld Y, Vervenne K, Arbocz J, et al. Multi-fidelity optimization of laminated conical shells for buckling[J]. Structural and Multidisciplinary Optimization, 2005, 30: 128-141, cited by 31. **Method**:Correction,response surfaces. **Fidelity Management**:No,**Discrete Fidelity: computer code STAGS-A, computer code BOCS. Optimization, application**: filament-wound laminated conical shells.

**Steady/Transient**

1. Guo Z, Song L, Park C, et al. Analysis of dataset selection for multi-fidelity surrogates for a turbine problem[J]. Structural and Multidisciplinary Optimization, 2018, 57: 2127-2142, cited by 44. **Method**:Co-kriging. **Fidelity Management**:No,**Discrete Fidelity:** Two unsteady Reynolds-averaged Navier-Stokes (RANS) equation solvers including (1) the full transient model (abbreviated as Transient) and (2) the transient rotor blade model with time transformation (abbreviated as TT), and (3) one steady RANS solver**, application**: two-variable turbine problem.
2. Mohammad Zadeh P, Mehmani A, Messac A. High fidelity multidisciplinary design optimization of a wing using the interaction of low and high fidelity models[J]. Optimization and Engineering, 2016, 17: 503-532.MLA, cited by 13. **Method**:Correction. **Fidelity Management**:No,**Discrete Fidelity: steady NavierStokes equations,**Reynolds-averaged Navier-Stokes (RANS) equations**, application**: Wortmann FX60.126 2D airfoil.
3. Giunta A A, Balabanov V, Kaufman M, et al. Variable-complexity response surface design of an HSCT configuration[J]. Multidisciplinary Design Optimization, Alexandrov NM and Hussaini MY eds, 1997, cited by 42. **Optimization, application**:aerodynamic-structural optimization of the High Speed Civil Transport (HSCT).
    
    [Problem ](https://www.notion.so/Problem-948b03cb331c4a468fe1594dda423e8c?pvs=21)
    
4. Meliani M, Bartoli N, Lefebvre T, et al. Multi-fidelity efficient global optimization: Methodology and application to airfoil shape design[C]//AIAA aviation 2019 forum. 2019: 3236, cited by 26.

### 7.2.2 electrode materials

1. Folch J P, Lee R M, Shafei B, et al. Combining multi-fidelity modelling and asynchronous batch Bayesian Optimization[J]. **`*Comput. Chem. Eng.*`**, 2023, cited by 7. **Method**:GP/MTGP. **Fidelity Management**:UCB/MES asynchronous batch. **Discrete Fidelity. Optimization, application**:electrode materials for optimal performance in pouch cells.

### 7.2.3 chemical reactor designs

1. Savage T, Basha N, Ehecatl O M, et al. Deep Gaussian Process-based Multi-fidelity Bayesian Optimization for Simulated Chemical Reactors,`*NeurIPS’22*`,2022, cited by 3.**Method**:DGP. **Fidelity Management**: UCB. **Discrete Fidelity. Optimization, application**: chemical reactor designs.
2. Savage T, Basha N, McDonough J, et al. Multi-Fidelity Data-Driven Design and Analysis of Reactor and Tube Simulations[J]. arXiv preprint `*arXiv*`, 2023, cited by 3. :GP. **Fidelity Management**: MES.  **Optimization, application**: chemical reactor designs.

### 7.2.2 Design

1. Li S, Xing W, Kirby R, et al. Multi-fidelity Bayesian optimization via deep neural networks[J]. `*NeurIPS’20*`, 2020, cited by 33. **Task**: Mechanical Plate Vibration Design, Thermal Conductor Design. **Fidelity type**: two fidelities, one with a coarse mesh and the other a dense mesh; mesh edge. **Method**: DNN. **Fidelity Management**: MES. **Discrete Fidelity.**
2. Haftka R T. Combining global and local approximations[J]. AIAA journal, 1991, 29(9): 1523-1525.

### Space infrastructure

Chen H, Sarton du Jonchay T, Hou L, et al. Multifidelity space mission planning and infrastructure design framework for space resource logistics[J]. Journal of Spacecraft and Rockets, 2021, 58(2): 538-551.

### Cooling hold design

[Applications   ](https://www.notion.so/000dce3472c4448d8654a21168633612?pvs=21)

## 7.3 Applications in Scientific Discovery

### 7.3.1 Applications of MFO in material science.

1. Wang Z, Liu X, Chen H, et al. Exploring Multi-Fidelity Data in Materials Science: Challenges, Applications, and Optimized Learning Strategies[J]. Applied Sciences, 2023, 13(24): 13176.
2. Liu X, De Breuck P P, Wang L, et al. A simple denoising approach to exploit multi-fidelity data for machine learning materials properties[J]. npj Computational Materials, 2022, 8(1): 233.
3. Clyde Fare, Peter Fenner, Matthew Benatan, Alessandro Varsi, and Edward O. Pyzer-Knapp. 2022. A multi-fidelity machine learning approach to high throughput materials screening. Npj Comput. Mater. 8 (2022), 1–9, cite by 7.
4. Mo C, Perdikaris P, Raney J R. Accelerated Design of Architected Materials with Multifidelity Bayesian Optimization[J]. Journal of Engineering Mechanics, 2023, 149(6): 04023032.
5. Tran A, Tranchida J, Wildey T, et al. Multi-fidelity machine-learning with uncertainty quantification and Bayesian optimization for materials design: Application to ternary random alloys[J]. The Journal of Chemical Physics, 2020, 153(7).

### 7.3.2 Applications of MFO in drug discovery.

1. **[IMPORTANT]** Buterez D, Janet J P, Kiddle S J, et al. MF-PCBA: Multifidelity High-Throughput Screening Benchmarks for Drug Discovery and Machine Learning[J]. Journal of Chemical Information and Modeling, 2023, 63(9): 2667-2678. cite by 4.
2. Buterez D, Janet J P, Kiddle S, et al. Multi-fidelity machine learning models for improved high-throughput screening predictions[J]. 2022.
3. Greenman K P, Green W H, Gómez-Bombarelli R. Multi-fidelity prediction of molecular optical peaks with deep learning[J]. Chemical science, 2022, 13(4): 1152-1162.
4. **[IMPORTANT]** Wu J, Wan Y, Wu Z, et al. MF-SuP-pKa: multi-fidelity modeling with subgraph pooling mechanism for pKa prediction[J]. Acta Pharmaceutica Sinica B, 2023, 13(6): 2572-2584.
5. Mayr, F., Wieder, M., Wieder, O. & Langer, T. Improving small molecule pka prediction using transfer learning with graph neural networks. Frontiers in
Chemistry 10 (2022).
6. **[IMPORTANT]** Madin O C, Shirts M R. Using physical property surrogate models to perform accelerated multi-fidelity optimization of force field parameters[J]. Digital Discovery, 2023.
    
    [](https://www.notion.so/adc1b02d00de4abb84f7eea81a91bdd4?pvs=21)
    
7. Hernandez-Garcia A, Saxena N, Jain M, et al. Multi-Fidelity Active Learning with GFlowNets[J]. arXiv preprint arXiv:2306.11715, 2023.
8. Egorova O, Hafizi R, Woods D C, et al. Multifidelity statistical machine learning for molecular crystal structure prediction[J]. The Journal of Physical Chemistry A, 2020, 124(39): 8065-8078.
    
    [](https://www.notion.so/9f608e70154047c2975df9ec9ec28acf?pvs=21)
    
9. Costabal F S, Matsuno K, Yao J, et al. Machine learning in drug development: characterizing the effect of 30 drugs on the QT interval using Gaussian process regression, sensitivity analysis, and uncertainty quantification[J]. Computer Methods in Applied Mechanics and Engineering, 2019, 348: 313-333.
10. Sahli Costabal F, Yao J, Kuhl E. Predicting the cardiac toxicity of drugs using a novel multiscale exposure–response simulator[J]. Computer methods in biomechanics and biomedical engineering, 2018, 21(3): 232-246.
11. Costabal F S, Yao J, Sher A, et al. Predicting critical drug concentrations and torsadogenic risk using a multiscale exposure-response simulator[J]. Progress in biophysics and molecular biology, 2019, 144: 61-76.
12. Sahli Costabal F, Yao J, Kuhl E. Predicting drug‐induced arrhythmias by multiscale modeling[J]. International journal for numerical methods in biomedical engineering, 2018, 34(5): e2964.
13. Duan Y J, Fu L, Zhang X C, et al. Improved GNNs for Log D 7.4 Prediction by Transferring Knowledge from Low-Fidelity Data[J]. Journal of Chemical Information and Modeling, 2023, 63(8): 2345-2359.
    
    [](https://www.notion.so/d599a2e724294e6c9575ffe42a928839?pvs=21)
    
14. Wang Y, Xiong J, Xiao F, et al. LogD7. 4 prediction enhanced by transferring knowledge from chromatographic retention time, microscopic pKa and logP[J]. Journal of Cheminformatics, 2023, 15(1): 76.
15. Zheng H, Luo W, Zhou G, et al. Uni-pKa: An Accurate and Physically Consistent pKa Prediction through Protonation Ensemble Modeling[J]. 2023.

---

# 8. MF review paper

## 8.1 MF model

1. **[IMPORTANT]** Fernández-Godino M G, Park C, Kim N H, et al. Review of multi-fidelity models[J]. `*arXiv*`, 2016, cited by 262. 
    
    [Detail](https://www.notion.so/Detail-f25d1a2c6478445591d3591a00ed072b?pvs=21)
    
2. **[IMPORTANT]** Park C, Haftka R T, Kim N H. Remarks on multi-fidelity surrogates[J]. `*Struct. Multidiscip. Optim.*`, 2017, 55: 1029-1050, cited by 179.
    
    [Detail ](https://www.notion.so/Detail-1a2a992ce41c4947ae71991e6bdf3d43?pvs=21)
    
3. **[IMPORTANT]** Fernández-Godino M G, Park C, Kim N H, et al. Review of Multi-Fidelity Surrogates; When Are They Worthwhile? 2018.
4. **[IMPORTANT]** Giselle Fernández-Godino M, Park C, Kim N H, et al. Issues in deciding whether to use multifidelity surrogates[J]. `*AIAA J.*`, 2019, 57(5): 2039-2054, cited by 144.
    
    [Detail ](https://www.notion.so/Detail-9468b6fd94aa48bc8fc3c18507f9a802?pvs=21)
    
5. **[IMPORTANT]** Brevault L, Balesdent M, Hebbal A. Overview of Gaussian process based multi-fidelity techniques with variable relationship between fidelities, application to aerospace systems[J]. **`*Aerosp. Sci. Technol.*`**, 2020, 107: 106339, cited by 30.
    
    [Detail ](https://www.notion.so/Detail-8c072c81182f4a318da09e65ef27218b?pvs=21)
    

## 8.2 MF optimization

1. **[IMPORTANT]** Peherstorfer B, Willcox K, Gunzburger M. Survey of multifidelity methods in uncertainty propagation, inference, and optimization[J]. `*SIAM REV.*`, 2018, 60(3): 550-591, cited by 808.
2. Zhou Q, Yang Y, Song X, et al. Survey of multi-fidelity surrogate models and their applications in the design and optimization of engineering equipment[J]. **`*J. Mech. Eng.*`**, 2020, 56(24): 219-245, cited by 11.
3. Biehler J, Mäck M, Nitzler J, et al. Multifidelity approaches for uncertainty quantification[J]. GAMM‐Mitteilungen, 2019, 42(2), cited by 10.

---

# 9. MF book

1. **[IMPORTANT]** Zhou Q, Zhao M, Hu J, et al. Multi-Fidelity Surrogates: Modeling, Optimization and Applications[M]. Springer, 2023.[https://link.springer.com/book/10.1007/978-981-19-7210-2](https://link.springer.com/book/10.1007/978-981-19-7210-2)
2. **[IMPORTANT]** Jiang P, Zhou Q, Shao X, et al. Surrogate-model-based design and optimization[M]. Springer Singapore, 2020, cited by 105.[https://link.springer.com/chapter/10.1007/978-981-15-0731-1_7](https://link.springer.com/chapter/10.1007/978-981-15-0731-1_7)
3. **[Uncertainty Analysis]** Mäck M. A Possibilistic Multifidelity Approach for the Uncertainty Analysis of Passive Safety Structures[M]. Shaker Verlag, 2021.[https://www.shaker.de/de/content/catalogue/index.asp?lang=de&ID=8&ISBN=978-3-8440-8034-6](https://www.shaker.de/de/content/catalogue/index.asp?lang=de&ID=8&ISBN=978-3-8440-8034-6)

---

# 10. MF Ph.D. Thesis

## 10.1 MF model

1. **[computer experiments ]** Le Gratiet L. Multi-fidelity Gaussian process regression for computer experiments[D]. Université Paris-Diderot-Paris VII, 2013, cited by 167.[https://theses.hal.science/file/index/docid/866770/filename/manuscrit.pdf](https://theses.hal.science/file/index/docid/866770/filename/manuscrit.pdf)
2. **[aerothermal analysis]** Santos M. Multi-fidelity modeling for aerothermal analysis of deployable planetary entry technologies[D]. Missouri University of Science and Technology, 2021.[https://scholarsmine.mst.edu/cgi/viewcontent.cgi?article=4021&context=doctoral_dissertations](https://scholarsmine.mst.edu/cgi/viewcontent.cgi?article=4021&context=doctoral_dissertations)
3. **[Encoder-Decoder Networks]** Partin L. Multitask and Multifidelity Convolutional Encoder-Decoder Networks[D]. University of Notre Dame, 2022.
4. **[simulation of wax deposition]** Farah Noroes Goncalves G. Multifidelity methods for simulation of wax deposition in single-phase and two-phase flow[D]. Imperial College London, 2023.[https://spiral.imperial.ac.uk/handle/10044/1/102792](https://spiral.imperial.ac.uk/handle/10044/1/102792)
5. **[风电场尾流场]** 王一妹.风电场尾流场与功率多精度模拟方法研究[D].2018.华北电力大学(北京), cited by 8.[http://cnki.cqgmy.edu.cn/KCMS/detail/detail.aspx?filename=1018241430.nh&dbcode=CDFD&dbname=CDFD2019](http://cnki.cqgmy.edu.cn/KCMS/detail/detail.aspx?filename=1018241430.nh&dbcode=CDFD&dbname=CDFD2019)

## 10.2 MF optimization

1. **[SBO]** Robinson T D. Surrogate-based optimization using multifidelity models with variable parameterization[D]. Massachusetts Institute of Technology, 2007, cited by 27.[https://dspace.mit.edu/bitstream/handle/1721.1/39666/176111691-MIT.pdf?sequence=2](https://dspace.mit.edu/bitstream/handle/1721.1/39666/176111691-MIT.pdf?sequence=2)
2. **[Aircraft Optimization** **]** Haas A. Multifidelity Optimization for Supersonic Aircraft Design[D]. Stanford University, 2012.
3. **[high-lift devicesn Optimization]** Demange J. Multifidelity multiobjective trust-region-based optimisation for high-lift devices[D]. , 2018, cited by 1.[https://dspace.lib.cranfield.ac.uk/bitstream/handle/1826/17783/Demange_J_2018.pdf?sequence=1&isAllowed=y](https://dspace.lib.cranfield.ac.uk/bitstream/handle/1826/17783/Demange_J_2018.pdf?sequence=1&isAllowed=y)
4. **[Uncertainty Quantification]** Masuda C M F. Multifidelity Methods for Uncertainty Quantification in Cardiovascular Hemodynamics[D]. Stanford University, 2022.
5. **[Multidisciplinary optimisation wing aerofoils]** Berci M. Multidisciplinary multifidelity optimisation of flexible wing aerofoils by passive adaptivity[D]. University of Leeds, 2011, cited by 1.
6. **[multidisciplinary system design]** March A I. Multidelity methods for multidisciplinary system design[D]. Massachusetts Institute of Technology, 2012, cited by 13.[https://dspace.mit.edu/bitstream/handle/1721.1/76145/820204781-MIT.pdf;sequence=2](https://dspace.mit.edu/bitstream/handle/1721.1/76145/820204781-MIT.pdf;sequence=2)
7. **[多层级筒壳屈曲分析及优化]** 田阔.基于多保真度建模的多层级筒壳屈曲分析及优化方法研究[D].2018.大连理工大学,cited by 9.
8. **[稳健性优化]** 张立丽.基于变可信度近似模型的序贯稳健性优化设计方法研究[D].2022.华中科技大学.
9. **[天线设计]** 姜宇虹.多精度数据驱动的昂贵优化问题求解及其在天线设计中的应用[D].2020.中国地质大学, cited by 1.

---

# 11. MF report

1. **[System-Level Engineering Analysis]** GARDNER D R, HENNIGAN G L. On Developing a Multifidelity Modeling Algorithm for System-Level Engineering Analysis[R]. Sandia National Lab.(SNL-NM), Albuquerque, NM (United States); Sandia National Lab.(SNL-CA), Livermore, CA (United States), 2003.[https://web.archive.org/web/20161227025614id_/http://prod.sandia.gov/techlib/access-control.cgi/2003/030399.pdf](https://web.archive.org/web/20161227025614id_/http://prod.sandia.gov/techlib/access-control.cgi/2003/030399.pdf)
2. **[Supersonic design]** Kroo I, Willcox K, March A, et al. Multifidelity analysis and optimization for supersonic design[R]. 2010, cited by 15.[https://ntrs.nasa.gov/api/citations/20100042294/downloads/20100042294.pdf](https://ntrs.nasa.gov/api/citations/20100042294/downloads/20100042294.pdf)
3. **[Optimization under Uncertainty]** Menhorn F, Geraci G, Seidl D T, et al. Multifidelity Monte Carlo Estimators for Robust Formulations in Optimization under Uncertainty[R]. Sandia National Lab.(SNL-NM), Albuquerque, NM (United States), 2021.[https://www.osti.gov/servlets/purl/1847580](https://www.osti.gov/servlets/purl/1847580)
4. **[Uncertainty Quantification]** Eldred M S, Monschke J A, Jakeman J D, et al. Multilevel-Multifidelity Approaches for Uncertainty Quantification and Design[R]. Sandia National Lab.(SNL-NM), Albuquerque, NM (United States), 2017.[https://www.osti.gov/servlets/purl/1455372](https://www.osti.gov/servlets/purl/1455372)
5. **[Uncertainty Quantification]** Geraci G, Eldred M S, Gorodetsky A, et al. Recent advancement in Multifidelity Uncertainty Quantification[R]. Sandia National Lab.(SNL-NM), Albuquerque, NM (United States), 2019.[https://www.osti.gov/servlets/purl/1642820](https://www.osti.gov/servlets/purl/1642820)

---

### 待看文献

**other Multi-fidelity model**

1. Jakeman J, Eldred M, Geraci G, et al. Multi-fidelity information fusion and resource allocation[R]. Sandia National Lab.(SNL-NM), Albuquerque, NM (United States), 2022.
2. Xu Y, Keshavarzzadeh V, Kirby R M, et al. A bandit-learning approach to multifidelity approximation[J]. SIAM Journal on Scientific Computing, 2022, 44(1): A150-A175.
3. Li K, He X, Lv L, et al. A Single-fidelity Surrogate Modeling Method based on Nonlinearity Integrated Multi-fidelity Surrogate[J]. `*J. Mech. Des.*`, 2023: 1-24.
4. Partin L, Geraci G, Rushdi A A, et al. Multifidelity data fusion in convolutional encoder/decoder networks[J]. **`*J. Comput. Phys.*`**, 2023, cited by 4.
5. Partin L. Multitask and Multifidelity Convolutional Encoder-Decoder Networks[M]. University of Notre Dame, 2022.
6. Partin L, Rushdi A A, Schiavazzi D E. Multifidelity data fusion in convolutional encoder/decoder assembly networks for computational fluid dynamics[C]//AIAA SCITECH 2022 Forum. 2022: 0803.
7. Conti P, Guo M, Manzoni A, et al. Multi-fidelity surrogate modeling using long short-term memory networks[J]. `*Comput. Methods Appl. Mech. Eng.*`, 2023, , cited by 6.
8. Wu D, Chinazzi M, Vespignani A, et al. Multi-fidelity hierarchical neural processes[C]//Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining. 2022, cited by 3.
9. Xiong F, Ren C, Mo B, et al. A new adaptive multi-fidelity metamodel method using meta-learning and Bayesian deep learning[J]. `*Struct. Multidiscip. Optim.*`, 2023, 66(3): 58.

**Aerodynamic Shape Optimization**

1. Yang A, Li J, Liem R P. Multi-fidelity Data-driven Aerodynamic Shape Optimization of Wings with Composite Neural Networks[C]//AIAA AVIATION 2023 Forum. 2023: 3470.下载不了
2. Nagy P, Jones B, Minisci E, et al. Multi-fidelity nonlinear aeroelastic analysis of a strut-braced ultra-high aspect ratio wing configuration[C]//AIAA AVIATION 2022 Forum. 2022: 3668.
3. Multi-fidelity model and reduced-order method for comprehensive hydrodynamic performance optimization and prediction of JBC ship
4. Towards multi-fidelity deep learning of wind turbine wakes
5. A Multi-Level, Multi-Scale Visual Analytics Approach to Assessment of Multifidelity HPC Systems
6. NM-MF: Non-Myopic Multifidelity Framework for Constrained Multi-Regime Aerodynamic Optimization

**Antenna Optimization**

1. Multi-fidelity Bayesian algorithm for antenna optimization
2. Pietrenko-Dabrowska A, Koziel S, Golunski L. Two-stage variable-fidelity modeling of antennas with domain confinement[J]. Scientific Reports, 2022, 12(1): 17275.

**Vehicle**

1. A multi-fidelity Gaussian process for efficient frequency sweeps in the acoustic design of a vehicle cabin
2. Physics-integrated Segmented Gaussian Process (SegGP) learning for cost-efficient training of diesel engine control system with low cetane numbers

**Hydrofoil**

1. Multi-fidelity hydrodynamic analysis of an autonomous surface vehicle at surveying speed in deep water subject to variable payload
2. Hydrofoil Optimization via Automated Multi-Fidelity Surrogate Models

**Shape Optimization**

1. Multi-fidelity Active Learning for Shape Optimization Problems Affected by Noise
2. Applications of multi-fidelity multi-output Kriging to engineering design optimization
3. Nonlinear Multi-Fidelity Bayesian Optimization: An Application in the Design of Blast Mitigating Structures 2022-01-0790
4. Zhang T, Barakos G N, Foster M. Multi-fidelity aerodynamic design and analysis of propellers for a heavy-lift eVTOL[J]. **`*Aerosp. Sci. Technol.*`**, 2023, , cited by 1.

**Cyber-Physical Systems**

1. Multi-fidelity Bayesian Optimization for Co-design of Resilient Cyber-Physical Systems

**digital twin**

1. Desai A S, Adhikari S, Chakraborty S. Enhanced multi-fidelity modelling for digital twin and uncertainty quantification[J]. arXiv preprint arXiv:2306.14430, 2023.

**Structural Health Monitoring**

1. A Multi-Fidelity Deep Neural Network Approach to Structural Health Monitoring 
2. A Machine Learning Framework for Physics-Based Multi-Fidelity Modeling and Health Monitoring for a Composite Wing
3. A Multi-Fidelity Deep Neural Network Approach to Structural Health Monitoring
4. A multi-fidelity surrogate model for structural health monitoring exploiting model order reduction and artificial neural networks

**Reinforcement Learning** 

1. Deep Reinforcement Learning for Robotic Control with Multi-Fidelity Models
2. Multi-fidelity reinforcement learning framework for shape optimization

**Transfer Learning**

1. Multi-Fidelity Transfer Learning for accurate database PDE approximation

uncertainty quantification

1. Multi-fidelity surrogate modeling adapted to functional outputs for uncertainty quantification of complex models
2. RMFGP: Rotated Multi-fidelity Gaussian process with Dimension Reduction for High-dimensional Uncertainty Quantification
3. Aerodynamic Shape Optimization Using Multi-fidelity Surrogate-based Approach for Computationally Expensive Problems
4. Quantitative Analysis of Nonlinear Multifidelity Optimization for Inverse Electrophysiology
5. Context-aware Budget-limited distribution learning in multifidelity problemslearning of hierarchies of low-fidelity models for multi-fidelity uncertainty quantification

**materials**

1. A multi-fidelity machine learning approach to high throughput materials screening
2. A simple denoising approach to exploit multi-fidelity data for machine learning materials properties
3. Yang Y, Eldred M S, Zádor J, et al. Multifidelity neural network formulations for prediction of reactive molecular potential energy surfaces[J]. Journal of Chemical Information and Modeling, 2023, 63(8): 2281-2295.

**Covalent Organic Frameworks**

1. Multi-fidelity Bayesian Optimization of Covalent Organic Frameworks for Xenon/Krypton Separations

**Biomanufacturing** 

1. Sun Y, Nathan-Roberts W, Pham T D, et al. Multi-fidelity Gaussian Process for Biomanufacturing Process Modeling with Small Data[J]. arXiv preprint arXiv:2211.14493, 2022.

**other**

1. Multifidelity validation of digital surrogates using variable-density turbulent mixing models
2. A novel fidelity selection strategy-guided multifidelity kriging algorithm for structural reliability analysis
3. A Deep Neural Network, Multi-fidelity Surrogate Model Approach for Bayesian Model Updating in SHM
4. Multi-fidelity optimization method with asynchronous generalized island model for AutoML
5. An approximate control variates approach to multifidelity distribution estimation
6. Improved multi-fidelity simulation-based optimisation: application in a digital twin shop floor
7. Multi-Fidelity Best-Arm Identification
8. Disentangled Multi-Fidelity Deep Bayesian Active Learning
9. Accelerated wind farm yaw and layout optimisation with multi-fidelity deep transfer learning wake models
10. Conglomerate Multi-Fidelity Gaussian Process Modeling, with Application to Heavy-Ion Collisions
11. Stacking designs: designing multi-fidelity experiments with target

[Thesis Planning](https://www.notion.so/Thesis-Planning-ea815ec7611e4d418b6e8885029fb562?pvs=21)
