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


## Setup

### Python

Supported Python Configurations:

| OS      | Python version |
| ------- | -------------- |
| macOS   | 3.7, 3.8, 3.9  |
| Ubuntu  | 3.7, 3.8, 3.9  |
| Windows | 3.7, 3.8, 3.9  |

### (Optional) Create a virtual environment

AIF360 requires specific versions of many Python packages which may conflict
with other projects on your system. A virtual environment manager is strongly
recommended to ensure dependencies may be installed safely. If you have trouble
installing AIF360, try this first.

#### Conda

Conda is recommended for all configurations though Virtualenv is generally
interchangeable for our purposes. [Miniconda](https://conda.io/miniconda.html)
is sufficient

Then, to create a new Python 3.9 environment, run:

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

### Install with `pip`

To install the latest stable version from PyPI, with complete functionality,  run:

```bash
pip install aif360[all]
```
If you encounter any errors, try the [Troubleshooting](#troubleshooting) steps.

#### Run the Examples

Finally, if you did not already, download the datasets as described in
[aif360/data/README.md](aif360/data/README.md).

### Troubleshooting

If you encounter any errors during the installation process, look for your
issue here and try the solutions.

## Using AIF360

The `examples` directory contains a diverse collection of jupyter notebooks
that use AI Fairness 360 in various ways. Both tutorials and demos illustrate
working code using AIF360. Tutorials provide additional discussion that walks
the user through the various steps of the notebook. See the details about
[tutorials and demos here](examples/README.md)

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
