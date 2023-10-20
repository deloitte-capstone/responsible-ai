# AI Fairness 360 (AIF360)

> See the original repository here: https://github.com/Trusted-AI/AIF360

The AI Fairness 360 toolkit is an extensible open-source library containing techniques developed by the
research community to help detect and mitigate bias in machine learning models throughout the AI application lifecycle. AI Fairness 360 package is available in both Python and R.

The AI Fairness 360 package includes
1) a comprehensive set of metrics for datasets and models to test for biases,
2) explanations for these metrics, and
3) algorithms to mitigate bias in datasets and models.
It is designed to translate algorithmic research from the lab into the actual practice of domains as wide-ranging
as finance, human capital management, healthcare, and education. AIF360 invites you to use it and improve it.

The [AI Fairness 360 interactive experience](https://aif360.res.ibm.com/data)
provides a gentle introduction to the concepts and capabilities. The [tutorials
and other notebooks](https://github.com/Trusted-AI/AIF360/tree/master/examples) offer a deeper, data scientist-oriented
introduction. The complete API is also available.

Being a comprehensive set of capabilities, it may be confusing to figure out
which metrics and algorithms are most appropriate for a given use case. To
help, AIF360 has created some [guidance
material](https://aif360.res.ibm.com/resources#guidance) that can be
consulted.

AIF360 has developed the package with extensibility in mind. This library is still
in development. AIF360 encourages the contribution of your metrics, explainers, and
debiasing algorithms.


## Setup (Python)

Supported Python Configurations:

| OS      | Python version |
| ------- | -------------- |
| macOS   | 3.8 – 3.11     |
| Ubuntu  | 3.8 – 3.11     |
| Windows | 3.8 – 3.11     |

### Step 1. Create a Virtual Environment

AIF360 requires specific versions of many Python packages which may conflict
with other projects on your system. A virtual environment manager is strongly
recommended to ensure dependencies may be installed safely.

#### 1a. Install Conda

Conda is recommended for all configurations though Virtualenv is generally
interchangeable for our purposes. [Miniconda](https://conda.io/miniconda.html)
is sufficient (see [the difference between Anaconda and
Miniconda](https://conda.io/docs/user-guide/install/download.html#anaconda-or-miniconda)
if you are curious) if you do not already have conda installed.

#### 1b. Create a new Python 3.11 virtual environment

To create a new Python 3.11 environment, run:

```bash
conda create --name aif360 python=3.11
conda activate aif360
```

The shell prompt should now begin with `(aif360) $`. To deactivate the environment, run:

```bash
(aif360) $ conda deactivate
```

The prompt will return to normal.

### Step 2. Install the AI Fairness 360 Package

#### 2a. Activate our `aif360` conda environment
First ensure you have activated the conda environment we created above:
```bash
conda activate aif360
```

#### 2b. Install the base AIF360 package
Use conda with the conda-forge channel to install AIF360:
```bash
conda install -y -c conda-forge aif360
```

### Step 3. Install All Other Packages

Now we want to install some additional dependencies that we'll use for exploration and specific algorithms. Such as Jupyter Lab to launch notebooks and the LIME package (Local Interpretable Model-agnostic Explanations) that we'll use to analyze our Medical Expenditure data later one.

#### 3a. Install dependencies
```bash
conda install -y -c conda-forge r-base cmake cvxpy
```

#### 3b. Install all optional AIF360 extras
```bash
pip install 'aif360[all]'
```

> **Note**\
> The requirements we need to conduct this replication are listed below. If you face issues during installation above, you can individually install these requirements -- if they all install successfully then you should be good to go!
> ```bash
> conda install -c conda-forge jupyterlab
> pip install xgboost
> pip install wrapt
> pip install fairlearn
> pip install BlackBoxAuditing
> pip install lime
> conda install -c conda-forge imbalanced-learn
> pip install statsmodels
> pip install shap
> ```

### Step 4. Test Our Installation and Start Using AIF360
The [`examples/` directory in the AIF360 repository](https://github.com/Trusted-AI/AIF360/tree/master/examples) contains a diverse collection of jupyter notebooks that use AI Fairness 360 in various ways. Both tutorials and demos illustrate working code using AIF360. Tutorials provide additional discussion that walks the user through the various steps of the notebook.

#### 4a. Fork the AIF360 Repository into your own GitHub Repo
- Fork the [AIF360 Repository](https://github.com/Trusted-AI/AIF360) into your own respective Repo
- Clone your forked repository to a local location where you can launch Jupyter Lab

#### 4b. Launch an example notebook
- With a shell open in the location where you cloned the repo, first activate the `aif360` conda environment then launch Jupyter Lab by running the following command:
  ```bash
  jupyter lab
  ```
- Open the `Bias Advertising` Jupyter [notebook](https://github.com/nanrahman/AIF360/blob/master/examples/tutorial_bias_advertising.ipynb)
- Follow instructions for downloading necessary data and run through the notebook

## Additional Info

### Citing AIF360

A technical description of AI Fairness 360 is available in this
[paper](https://arxiv.org/abs/1810.01943). Below is the bibtex entry for this
paper.

```
@misc{aif360-oct-2018,
    title = "{AI Fairness} 360:  An Extensible Toolkit for Detecting, Understanding, and Mitigating Unwanted Algorithmic Bias",
    author = {Rachel K. E. Bellamy and Kuntal Dey and Michael Hind and
	Samuel C. Hoffman and Stephanie Houde and Kalapriya Kannan and
	Pranay Lohia and Jacquelyn Martino and Sameep Mehta and
	Aleksandra Mojsilovic and Seema Nagar and Karthikeyan Natesan Ramamurthy and
	John Richards and Diptikalyan Saha and Prasanna Sattigeri and
	Moninder Singh and Kush R. Varshney and Yunfeng Zhang},
    month = oct,
    year = {2018},
    url = {https://arxiv.org/abs/1810.01943}
}
```

### AIF360 Videos

* Introductory [video](https://www.youtube.com/watch?v=X1NsrcaRQTE) to AI
  Fairness 360 by Kush Varshney, September 20, 2018 (32 mins)

### Supported bias mitigation algorithms and fairness metrics

<details><summary>View all</summary>

#### Supported bias mitigation algorithms

* Optimized Preprocessing ([Calmon et al., 2017](http://papers.nips.cc/paper/6988-optimized-pre-processing-for-discrimination-prevention))
* Disparate Impact Remover ([Feldman et al., 2015](https://doi.org/10.1145/2783258.2783311))
* Equalized Odds Postprocessing ([Hardt et al., 2016](https://papers.nips.cc/paper/6374-equality-of-opportunity-in-supervised-learning))
* Reweighing ([Kamiran and Calders, 2012](http://doi.org/10.1007/s10115-011-0463-8))
* Reject Option Classification ([Kamiran et al., 2012](https://doi.org/10.1109/ICDM.2012.45))
* Prejudice Remover Regularizer ([Kamishima et al., 2012](https://rd.springer.com/chapter/10.1007/978-3-642-33486-3_3))
* Calibrated Equalized Odds Postprocessing ([Pleiss et al., 2017](https://papers.nips.cc/paper/7151-on-fairness-and-calibration))
* Learning Fair Representations ([Zemel et al., 2013](http://proceedings.mlr.press/v28/zemel13.html))
* Adversarial Debiasing ([Zhang et al., 2018](https://arxiv.org/abs/1801.07593))
* Meta-Algorithm for Fair Classification ([Celis et al., 2018](https://arxiv.org/abs/1806.06055))
* Rich Subgroup Fairness ([Kearns, Neel, Roth, Wu, 2018](https://arxiv.org/abs/1711.05144))
* Exponentiated Gradient Reduction ([Agarwal et al., 2018](https://arxiv.org/abs/1803.02453))
* Grid Search Reduction ([Agarwal et al., 2018](https://arxiv.org/abs/1803.02453), [Agarwal et al., 2019](https://arxiv.org/abs/1905.12843))
* Fair Data Adaptation ([Plečko and Meinshausen, 2020](https://www.jmlr.org/papers/v21/19-966.html), [Plečko et al., 2021](https://arxiv.org/abs/2110.10200))
* Sensitive Set Invariance/Sensitive Subspace Robustness ([Yurochkin and Sun, 2020](https://arxiv.org/abs/2006.14168), [Yurochkin et al., 2019](https://arxiv.org/abs/1907.00020))

#### Supported fairness metrics

* Comprehensive set of group fairness metrics derived from selection rates and error rates including rich subgroup fairness
* Comprehensive set of sample distortion metrics
* Generalized Entropy Index ([Speicher et al., 2018](https://doi.org/10.1145/3219819.3220046))
* Differential Fairness and Bias Amplification ([Foulds et al., 2018](https://arxiv.org/pdf/1807.08362))
* Bias Scan with Multi-Dimensional Subset Scan ([Zhang, Neill, 2017](https://arxiv.org/abs/1611.08292))

</details>
