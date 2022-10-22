# AI Fairness 360 (AIF360)

[![Continuous Integration](https://github.com/Trusted-AI/AIF360/actions/workflows/ci.yml/badge.svg)](https://github.com/Trusted-AI/AIF360/actions/workflows/ci.yml)
[![Documentation](https://readthedocs.org/projects/aif360/badge/?version=latest)](http://aif360.readthedocs.io/en/latest/?badge=latest)
[![PyPI version](https://badge.fury.io/py/aif360.svg)](https://badge.fury.io/py/aif360)
[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/aif360)](https://cran.r-project.org/package=aif360)

The AI Fairness 360 toolkit is an extensible open-source library containing techniques developed by the
research community to help detect and mitigate bias in machine learning models throughout the AI application lifecycle. AI Fairness 360 package is available in both Python and R.

The AI Fairness 360 package includes
1) a comprehensive set of metrics for datasets and models to test for biases,
2) explanations for these metrics, and
3) algorithms to mitigate bias in datasets and models.
It is designed to translate algorithmic research from the lab into the actual practice of domains as wide-ranging
as finance, human capital management, healthcare, and education. AIF360 invites you to use it and improve it.

The [AI Fairness 360 interactive experience](http://aif360.mybluemix.net/data)
provides a gentle introduction to the concepts and capabilities. The [tutorials
and other notebooks](./examples) offer a deeper, data scientist-oriented
introduction. The complete API is also available.

Being a comprehensive set of capabilities, it may be confusing to figure out
which metrics and algorithms are most appropriate for a given use case. To
help, AIF360 have created some [guidance
material](http://aif360.mybluemix.net/resources#guidance) that can be
consulted.

AIF360 has developed the package with extensibility in mind. This library is still
in development. AIF360 encourages the contribution of your metrics, explainers, and
debiasing algorithms.


# Setup (Python)

Supported Python Configurations:

| OS      | Python version |
| ------- | -------------- |
| macOS   | 3.7, 3.8, 3.9  |
| Ubuntu  | 3.7, 3.8, 3.9  |
| Windows | 3.7, 3.8, 3.9  |

##  Step 1:Create a virtual environment
AIF360 requires specific versions of many Python packages which may conflict
with other projects on your system. A virtual environment manager is strongly
recommended to ensure dependencies may be installed safely.

### 1a: Install Conda
Conda is recommended for all configurations though Virtualenv is generally
interchangeable for our purposes. [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
is sufficient, please refer to the link for installing on your operation system. 

### 1b: Create a new Python 3.9 virtual environment. 
Activate conda and run:

```bash
conda create --name aif360 python=3.9
conda activate aif360
```
The shell should now look like `(aif360) $`. To deactivate the environment, run:

```bash
(aif360)$ conda deactivate
```
The prompt will return to `$ `.
Note: Older versions of conda may use `source activate aif360` and `source
deactivate` (`activate aif360` and `deactivate` on Windows).

## Step 2: Install AIFairness 360 Package

### 2a: Ensure conda is running, now initialize your `aif360` conda environment.
Refer to the [Conda User Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/index.html), 
which includes a good walkthrough on how to use.

### 2b: Install AIF360 with `pip`
With your `aif360` environment running, install the latest stable version from PyPI.
To install with complete functionality,  run:

```bash
pip install 'aif360[all]'
```
### Step 3: Install Jupyter Lab

```bash
conda install -c conda-forge jupyterlab
```
Once installed, to run Jupyter enter the following (ensuring you are in your aif360 env)

```bash
jupyter-lab
```
Refer to `Getting Started` and `User Guide` documentation on [Jupyter Notebooks](https://jupyterlab.readthedocs.io/en/stable/)for information on how to use.

### Step 4: Install other packages
**Note:** these requirements may already be satisfied by AIF360, but just in case we list them here for install. 

```bash
pip install xgboost
pip install wrapt
pip install fairlearn
pip install BlackBoxAuditing
pip install lime
conda install -c conda-forge imbalanced-learn
pip install statsmodels
pip install shap
```

## Step 5: Test out install and using AIF360
The `examples` directory in the [AIF360 Repository](https://github.com/Trusted-AI/AIF360/tree/master/examples) 
contains a diverse collection of jupyter notebooks that use AI Fairness 360 in various ways. Both tutorials and demos illustrate
working code using AIF360. Tutorials provide additional discussion that walks the user through the various steps of the notebook. See the details about [AIF360](https://github.com/Trusted-AI/AIF360) in their central repository.

### Step 5a: Fork the AIF360 Repository into your own GitHub Repo
* Fork the AIF360 [Repository](https://github.com/Trusted-AI/AIF360) in your own respective Repo
* Clone your forked repository to a local location so you can launch Jupyter labs

### Step 5b: Launch an example notebook
* Launch the `Bias Advertising` Jupyter [notebook](https://github.com/nanrahman/AIF360/blob/master/examples/tutorial_bias_advertising.ipynb)
* Follow instructions for downloading necessary data and run notebook

## Citing AIF360

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

## AIF360 Videos

* Introductory [video](https://www.youtube.com/watch?v=X1NsrcaRQTE) to AI
  Fairness 360 by Kush Varshney, September 20, 2018 (32 mins)

## Contributing
The development fork for Rich Subgroup Fairness (`inprocessing/gerryfair_classifier.py`) is [here](https://github.com/sethneel/aif360). Contributions are welcome and a list of potential contributions from the authors can be found [here](https://trello.com/b/0OwPcbVr/gerryfair-development).
