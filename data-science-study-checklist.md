# Study checklist for a beginner data scientist

I recently met someone who wants to learn how to do data-science - like I did years ago! So I briefly thought about what advice should I give her, and came up with this list of topics a budding data-scientist should know. 



This list isn't exhaustive - there are other things you will want to learn, as you progress in the field and search for your niche. It also doesn't show you the only learning path that will make you a data-scientist. It also doesn't contain learning resources, because the net is full of them. It's just a guide for your self-study, until you can guide it yourself.



### Legend

- :small_blue_diamond::small_blue_diamond::small_blue_diamond: know this well, it will be your bread and butter

- :small_blue_diamond::small_blue_diamond: know this well enough so that at worst, you need to google some specifics

- :small_blue_diamond:know that this exists and what it is, you will learn the details later as you need them

## Basic tools

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:vscode - IDE, or other IDE of your choice
- :small_blue_diamond::small_blue_diamond::small_blue_diamond:jupyter notebooks - code format and editor good for interactive data exploration and visualisation. Compatible with both vscode and Google Collab
- :small_blue_diamond::small_blue_diamond::small_blue_diamond:basics of work with Linux terminal (or Windows command line)- change directory, list its contents, run a command, display help for the command
- :small_blue_diamond::small_blue_diamond:git
- :small_blue_diamond::small_blue_diamond:GitHub (or GitLab, Gitea or similar)

## Programming

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:Python
- :small_blue_diamond:Sql

## Data formats

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:CSV - basic format for tabular data, compatible with Excel 
- :small_blue_diamond::small_blue_diamond:JSON -  widespread format, can handle non-tabular data. Also check out jq for JSON exploration

## Python packages and tools

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:Pandas - general, high level work with tables, python equivalent of Excel. Learn to load data, transform it and select some parts of it, the rest is optional.

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:Matplotlib - most widespread data plotting package, used also by Pandas and Scikit-learn. Learn how to do basic plots, the rest is optional.

- :small_blue_diamond:Seaborn - very usefull extension of matplotlib capabilities, it's a good idea to get used to it for basic plots instead of matplotlib.

- :small_blue_diamond::small_blue_diamond:Numpy - matrix multiplication and other linear algebra, work with numerical arrays

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:Scikit-learn - huge collection of models and tools for model evaluation, from basic to advanced. Learn where the model performance evaluation tools are, learn what the model interface looks like, treat the list of available models as a learning checklist for further study.

- :small_blue_diamond:Scipy - advanced mathematics, statistics and optimisation

- :small_blue_diamond:Pytorch and/or Tensorflow - python packages for neural networks

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:pip package manager - you will need it to install all these packages anyway

- :small_blue_diamond:conda package manager and virtual environment

## Math

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:Linear algebra - :small_blue_diamond::small_blue_diamond::small_blue_diamond:vectors, :small_blue_diamond::small_blue_diamond::small_blue_diamond:matrix multiplication, :small_blue_diamond:geometric interpretation
- :small_blue_diamond::small_blue_diamond::small_blue_diamond:Basics of statistics - :small_blue_diamond::small_blue_diamond::small_blue_diamond:probability, :small_blue_diamond::small_blue_diamond::small_blue_diamond:probability distribution, :small_blue_diamond::small_blue_diamond:conditional probabiliy,:small_blue_diamond::small_blue_diamond:confidence interval, :small_blue_diamond:what is a statistical test, :small_blue_diamond::small_blue_diamond::small_blue_diamond:Normal distribution, :small_blue_diamond::small_blue_diamond:Binomial distribution , :small_blue_diamond::small_blue_diamond:Poisson distribution, :small_blue_diamond::small_blue_diamond:Correlation, :small_blue_diamond::small_blue_diamond::small_blue_diamond:Categorical distribution
- :small_blue_diamond::small_blue_diamond:Simpsons paradox, :small_blue_diamond::small_blue_diamond:Selection bias, :small_blue_diamond::small_blue_diamond:Survivor bias, :small_blue_diamond::small_blue_diamond::small_blue_diamond:Confounding variable and spurrious correlation 
- :small_blue_diamond:Unintuitive properties of high dimensional spaces
- :small_blue_diamond:Intro to Bayesian statistics - Bayes rule, apriori and aposteriori probability distribution. Maximum likelihood and maximum aposteriori estimates.

## Modeling

- :small_blue_diamond::small_blue_diamond::small_blue_diamond:regression Vs classification
- :small_blue_diamond::small_blue_diamond::small_blue_diamond:linear regression and logistic regression
- :small_blue_diamond::small_blue_diamond::small_blue_diamond:overfitting and strategies against it -> :small_blue_diamond::small_blue_diamond::small_blue_diamond:train/test/validation split or :small_blue_diamond::small_blue_diamond:crossvalidation, :small_blue_diamond::small_blue_diamond:regularisation, :small_blue_diamond:data augmentation
- :small_blue_diamond::small_blue_diamond:data normalisation - which models need it, which are immune
- :small_blue_diamond::small_blue_diamond::small_blue_diamond:confusion matrix - recall (sensitivity), precision, specificity, accuracy and tradeoffs between them.
- :small_blue_diamond::small_blue_diamond:roc curve, roc auc score (perhaps also precision-recall curve)
- :small_blue_diamond:data imbalance - what problems can it cause?
- :small_blue_diamond::small_blue_diamond:decision boundary, linear Vs non linear models - what is a linearly separable data?
- :small_blue_diamond:Feature engineering (a.k.a kernels) for turning linear models non-linear
- :small_blue_diamond::small_blue_diamond:Decision tree
- :small_blue_diamond:Neural networks for classification
- :small_blue_diamond:Bias Vs variance tradeoff
- :small_blue_diamond:Ensemble models
- :small_blue_diamond:Clustering
- :small_blue_diamond:Topic modeling
- :small_blue_diamond:Dimensionality reduction
- :small_blue_diamond:Autencoder - what is embedding?

## Ethics

- Biased data leads to  biased models
- Misinterpretation of model output meaning - The user doesn't understand the math as you do.
- Overestimation of model output reliability - The user doesn't understand the limitations of the model as you do.
- Unintended use - users do whatever they want, sometimes it's great, but sometimes it's stupid and sometimes it's evil.
- Automated decision making - don't do it, it's better to assist human decision makers, but keep in mind previous bullet points.
- When not to do machine learning - good UI and good math are often a better solution than a good model



## What does usual data-scientist workflow look like?

- Load data
- Explore it - what does it look like, how much is there, what data is missing, is it biased in some way? What data do you actually need? Are there outliers? Visualise it to get a better feel for it.
- Compute metrics you care about (means, medians, variance, correlation and rank correlation)
- Remove duplicates, deal with missing data, decide what to do with outliers
- Model the data - understand what answer you want and what type of model can give you that
- Evaluate your model - does it do what you want? If not, return to previous step.
- Visualise and clearly communicate the conclusions of your modeling - what do they mean? How certain are you?
- If needed, deploy the model for repeated use
