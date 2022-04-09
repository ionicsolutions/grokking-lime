# Grokking LIME: How can we explain why an image classifier "knows" what’s in a photo without looking inside the model?

Kilian Kluge @ PyConDE & PyData Berlin 2022, [April 12th 2022, 15:30, A1](https://2022.pycon.de/program/ZJUWZJ/)

## Abstract

Machine learning models show outstanding performance at many tasks. 
But it often remains a mystery to their users how they arrived at their predictions.
This quickly becomes a problem in application settings where “The computer says so!” is not a sufficient explanation.

LIME is one of the most widely-known algorithms for explaining black-box models.
First published in 2016, it has helped popularize the concept of “model-agnostic” explanations
and inspired subsequent developments.
Thus, it’s an approach worth understanding and an excellent starting point for exploring
interpretable machine learning.

In this talk, to truly grok how LIME generates its explanations, we will implement the algorithm from scratch.
Starting with nothing but an image file and a machine learning model, we will work through the six 
steps necessary to generate visual explanations.

Along the way, we will discuss the “Four Principles for Explainable AI” published by NIST in the fall of 2021.
These human-centered principles provide a practical guideline for designing and implementing explanations
for machine learning models.

Don’t worry: No knowledge of machine learning is required to follow this talk. 
Aside from familiarity with the basics of `numpy` arrays, all you need is your curiosity.

## Instructions

As (almost) always, it's best to create a fresh, clean Python environment for the _Grokking LIME_ tutorial.
This will ensure that there are no strange dependency conflicts.

If you don't know how to do that, you can follow
[this tutorial](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
to learn more about virtual environments.
Or, just run the following commands in your terminal to create a new virtual environment and activate it:
```shell
$ python3 -m pip install --upgrade pip
$ python3 -m pip install virtualenv
$ python3 -m venv env
$ source env/bin/activate
```

Next, clone the repository and install the required dependencies:
```shell
$ git clone https://github.com/ionicsolutions/grokking-lime
$ cd grokking-lime
$ pip install -r requirements.txt 
```

Then, you can launch the Jupyter notebook server:
```shell
$ jupyter notebook
```

After clicking the link that Jupyter generates, you'll find the completed tutorial in
[grokking-lime-complete.ipynb](./grokking-lime-complete.ipynb)
and the version to code along with in
[grokking-lime.ipynb](./grokking-lime.ipynb).

## Links & further reading

- Papers:
  - Phillips et al. (2021): [Four Principles of Explainable AI](https://nvlpubs.nist.gov/nistpubs/ir/2021/NIST.IR.8312.pdf) (NIST)
  - Ribeiro et al. (2016): ["Why Should I Trust You?": Explaining the Predictions of Any Classifier](https://arxiv.org/abs/1602.04938)
- LIME implementations:
  - [Original LIME on GitHub](https://github.com/marcotcr/lime) & [on PyPI](https://pypi.org/project/lime/)
  - [VisuaLIME on GitHub](https://github.com/xai-demonstrator/visualime) & [on PyPI](https://pypi.org/project/visualime/)
- Affiliations:
  - [Inlinity](https://www.inlinity.ai) ([LinkedIn](https://www.linkedin.com/company/inlinity/))
  - [XAI Studio](https://www.xai-studio.de) ([LinkedIn](https://www.linkedin.com/company/xai-studio/))