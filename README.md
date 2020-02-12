Feature-Engineering-Handbook
============
Welcome! This repo provides an interactive and complete practical feature engineering tutorial in Jupyter Notebook. It contains three parts: [Data Prepocessing](1.%20Data%20Preprocessing.ipynb), [Feature Selection](2.%20Feature%20Selection.ipynb) and [Dimension Reduction](3.%20Dimension%20Reduction.ipynb). Each part is demonstrated separately in one notebook. Since some feature selection algorithms such as Simulated Annealing and Genetic Algorithm lack complete implementation in python, we also provide corresponding python scripts ([Simulated Annealing](SA.py), [Genetic Algorithm](GA.py)) and cover them in our tutorial for your reference. 


Brief Introduction
------------
- [Notebook One](1.%20Data%20Preprocessing.ipynb) covers data preprocessing on static continuous features based on [scikit-learn](https://scikit-learn.org/stable/), on static categorical features based on [Category Encoders](https://contrib.scikit-learn.org/categorical-encoding/), and on time series features based on [Featuretools](https://www.featuretools.com/).  
  
- [Notebook Two](2.%20Feature%20Selection.ipynb) covers feature selection including univariate filter methods based on [scikit-learn](https://scikit-learn.org/stable/), multivariate filter methods based on [scikit-feature](http://featureselection.asu.edu/), deterministic wrapper methods based on [scikit-learn](https://scikit-learn.org/stable/), randomized wrapper methods based on our implementations in python scrips, and embedded methods based on [scikit-learn](https://scikit-learn.org/stable/).
  
- [Notebook Three](3.%20Dimension%20Reduction.ipynb) covers supervised and unsupervised dimension reduction based on [scikit-learn](https://scikit-learn.org/stable/).


Table of Content
------------
<div class="toc"><ul class="toc-item"><li><span><span class="toc-item-num">1&nbsp;&nbsp;</span>Data Prepocessing</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.1&nbsp;&nbsp;</span>Static Continuous Variables</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.1.1&nbsp;&nbsp;</span>Discretization</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.1.1.1&nbsp;&nbsp;</span>Binarization</a></span></li><li><span><span class="toc-item-num">1.1.1.2&nbsp;&nbsp;</span>Binning</a></span></li></ul></li><li><span><span class="toc-item-num">1.1.2&nbsp;&nbsp;</span>Scaling</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.1.2.1&nbsp;&nbsp;</span>Stardard Scaling (Z-score standardization)</a></span></li><li><span><span class="toc-item-num">1.1.2.2&nbsp;&nbsp;</span>MinMaxScaler (Scale to range)</a></span></li><li><span><span class="toc-item-num">1.1.2.3&nbsp;&nbsp;</span>RobustScaler (Anti-outliers scaling)</a></span></li><li><span><span class="toc-item-num">1.1.2.4&nbsp;&nbsp;</span>Power Transform (Non-linear transformation)</a></span></li></ul></li><li><span><span class="toc-item-num">1.1.3&nbsp;&nbsp;</span>Normalization</a></span></li><li><span><span class="toc-item-num">1.1.4&nbsp;&nbsp;</span>Imputation of missing values</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.1.4.1&nbsp;&nbsp;</span>Univariate feature imputation</a></span></li><li><span><span class="toc-item-num">1.1.4.2&nbsp;&nbsp;</span>Multivariate feature imputation</a></span></li><li><span><span class="toc-item-num">1.1.4.3&nbsp;&nbsp;</span>Marking imputed values</a></span></li></ul></li><li><span><span class="toc-item-num">1.1.5&nbsp;&nbsp;</span>Feature Transformation</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.1.5.1&nbsp;&nbsp;</span>Polynomial Transformation</a></span></li><li><span><span class="toc-item-num">1.1.5.2&nbsp;&nbsp;</span>Custom Transformation</a></span></li></ul></li></ul></li><li><span><span class="toc-item-num">1.2&nbsp;&nbsp;</span>Static Categorical Variables</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.2.1&nbsp;&nbsp;</span>Ordinal Encoding</a></span></li><li><span><span class="toc-item-num">1.2.2&nbsp;&nbsp;</span>One-hot Encoding</a></span></li><li><span><span class="toc-item-num">1.2.3&nbsp;&nbsp;</span>Hashing Encoding</a></span></li><li><span><span class="toc-item-num">1.2.4&nbsp;&nbsp;</span>Helmert Coding</a></span></li><li><span><span class="toc-item-num">1.2.5&nbsp;&nbsp;</span>Sum (Deviation) Coding</a></span></li><li><span><span class="toc-item-num">1.2.6&nbsp;&nbsp;</span>Target Encoding</a></span></li><li><span><span class="toc-item-num">1.2.7&nbsp;&nbsp;</span>M-estimate Encoding</a></span></li><li><span><span class="toc-item-num">1.2.8&nbsp;&nbsp;</span>James-Stein Encoder</a></span></li><li><span><span class="toc-item-num">1.2.9&nbsp;&nbsp;</span>Weight of Evidence Encoder</a></span></li><li><span><span class="toc-item-num">1.2.10&nbsp;&nbsp;</span>Leave One Out Encoder</a></span></li><li><span><span class="toc-item-num">1.2.11&nbsp;&nbsp;</span>Catboost Encoder</a></span></li></ul></li><li><span><span class="toc-item-num">1.3&nbsp;&nbsp;</span>Time Series Variables</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.3.1&nbsp;&nbsp;</span>Time Series Categorical Features</a></span></li><li><span><span class="toc-item-num">1.3.2&nbsp;&nbsp;</span>Time Series Continuous Features</a></span></li><li><span><span class="toc-item-num">1.3.3&nbsp;&nbsp;</span>Implementation</a></span><ul class="toc-item"><li><span><span class="toc-item-num">1.3.3.1&nbsp;&nbsp;</span>Create EntitySet</a></span></li><li><span><span class="toc-item-num">1.3.3.2&nbsp;&nbsp;</span>Set up cut-time</a></span></li><li><span><span class="toc-item-num">1.3.3.3&nbsp;&nbsp;</span>Auto Feature Engineering</a></span></li></ul></li></ul></li></ul></li><li><span><span class="toc-item-num">2&nbsp;&nbsp;</span>Feature Selection</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.1&nbsp;&nbsp;</span>Filter Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.1.1&nbsp;&nbsp;</span>Univariate Filter Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.1.1.1&nbsp;&nbsp;</span>Variance Threshold</a></span></li><li><span><span class="toc-item-num">2.1.1.2&nbsp;&nbsp;</span>Pearson Correlation (regression problem)</a></span></li><li><span><span class="toc-item-num">2.1.1.3&nbsp;&nbsp;</span>Distance Correlation (regression problem)</a></span></li><li><span><span class="toc-item-num">2.1.1.4&nbsp;&nbsp;</span>F-Score (regression problem)</a></span></li><li><span><span class="toc-item-num">2.1.1.5&nbsp;&nbsp;</span>Mutual Information (regression problem)</a></span></li><li><span><span class="toc-item-num">2.1.1.6&nbsp;&nbsp;</span>Chi-squared Statistics (classification problem)</a></span></li><li><span><span class="toc-item-num">2.1.1.7&nbsp;&nbsp;</span>F-Score (classification problem)</a></span></li><li><span><span class="toc-item-num">2.1.1.8&nbsp;&nbsp;</span>Mutual Information (classification problem)</a></span></li></ul></li><li><span><span class="toc-item-num">2.1.2&nbsp;&nbsp;</span>Multivariate Filter Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.1.2.1&nbsp;&nbsp;</span>Max-Relevance Min-Redundancy (mRMR)</a></span></li><li><span><span class="toc-item-num">2.1.2.2&nbsp;&nbsp;</span>Correlation-based Feature Selection (CFS)</a></span></li><li><span><span class="toc-item-num">2.1.2.3&nbsp;&nbsp;</span>Fast Correlation-based Filter (FCBF)</a></span></li><li><span><span class="toc-item-num">2.1.2.4&nbsp;&nbsp;</span>ReliefF</a></span></li><li><span><span class="toc-item-num">2.1.2.5&nbsp;&nbsp;</span>Spectral Feature Selection (SPEC)</a></span></li></ul></li></ul></li><li><span><span class="toc-item-num">2.2&nbsp;&nbsp;</span>Wrapper Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.2.1&nbsp;&nbsp;</span>Deterministic Algorithms</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.2.1.1&nbsp;&nbsp;</span>Recursive Feature Elimination (SBS)</a></span></li></ul></li><li><span><span class="toc-item-num">2.2.2&nbsp;&nbsp;</span>Randomized Algorithms</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.2.2.1&nbsp;&nbsp;</span>Simulated Annealing (SA)</a></span></li><li><span><span class="toc-item-num">2.2.2.2&nbsp;&nbsp;</span>Genetic Algorithm (GA)</a></span></li></ul></li></ul></li><li><span><span class="toc-item-num">2.3&nbsp;&nbsp;</span>Embedded Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.3.1&nbsp;&nbsp;</span>Regulization Based Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">2.3.1.1&nbsp;&nbsp;</span>Lasso Regression (Linear Regression with L1 Norm)</a></span></li><li><span><span class="toc-item-num">2.3.1.2&nbsp;&nbsp;</span>Logistic Regression (with L1 Norm)</a></span></li><li><span><span class="toc-item-num">2.3.1.3&nbsp;&nbsp;</span>LinearSVR/ LinearSVC</a></span></li></ul></li><li><span><span class="toc-item-num">2.3.2&nbsp;&nbsp;</span>Tree Based Methods</a></span></li></ul></li></ul></li><li><span><span class="toc-item-num">3&nbsp;&nbsp;</span>Dimension Reduction</a></span><ul class="toc-item"><li><span><span class="toc-item-num">3.1&nbsp;&nbsp;</span>Unsupervised Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">3.1.1&nbsp;&nbsp;</span>PCA (Principal Components Analysis)</a></span></li></ul></li><li><span><span class="toc-item-num">3.2&nbsp;&nbsp;</span>Supervised Methods</a></span><ul class="toc-item"><li><span><span class="toc-item-num">3.2.1&nbsp;&nbsp;</span>LDA (Linear Discriminant Analysis)</a></span></li></ul></li></ul></li></ul></div>

Reference
------------
References have been included in each Jupyter Notebooks.

Author
------------
[**@Yingxiang Chen**](https://github.com/YC-Coder-Chen)  
[**@Zihan Yang**](https://github.com/echoyang48)

Contact
------------
**If there are any mistakes, please feel free to reach out and correct us!**  

Yingxiang Chen E-mail: chenyingxiang3526@gmail.com  
Zihan Yang E-mai: echoyang48@gmail.com
