---
title: Setting Up Your Workspace II
subtitle: Coding Environments
date: 2022-05-27T09:07:56.927Z
summary: We continue the second part of Setting up the workspace with a few tips
  and links to getting templates and structures for various development
  projects.
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
The first part of this article was focused on the idea of making the directories follow a structure that makes it easy to:

* replicate file structures for various tasks
* find and locate files and directories easily
* optimise time spent on work or computer related tasks
* make memory allocation on the computer efficient
* motivate you to work when you sit down at you computer
* declutter your life

This second part continues with the idea but is focused more on setting up work environments for projects related to coding and data science. This forms an important part of working in a development environment.

Picture this, the priest always has his stole, a bottle of holy water and chrism oil in the little box he has wherever he is going. The soldier has his arms. The artist is never found without a pencil and sketchpad, nor a tailor without his tape rule.

So too should the software engineer, software developer or data scientist always be fitted with the right tools for work. The major tools are the project templates and the git or version control system. Project templates are default files and directory structures that are put in place for all the different kinds of projects you might potentially work on. They could be R, Python, Ruby, Django, Go, Flask, C++, you name it.

The template has the various files that every project needs in order to work well. Pre-populating a project directory with the template makes it possible to automate the file structure required in setting up a development project in whatever language you work with, or on whatever kind of task you work on. That means that you can design your project by either programming language or task. With this you can have either a Data science template, Python template, or as many templates as you need for the different kinds of projects you are working on.

**Advantages:**

The advantages are similar to those of having a file or directory structure but you can also add a few more.

* reproducibility
* shareability
* reusability

Several tools exist for creating project templates that anyone can use for their software projects. Some of the ones I found include [Cookiecutter for Python Projects](https://cookiecutter.readthedocs.io/en/latest/tutorial1.html#step-1-generate-a-python-package-project), [Cookiecutter for Data Science](https://drivendata.github.io/cookiecutter-data-science/), [Project R](http://projecttemplate.net/index.html), [Django](http://projecttemplate.net/index.html), and [Flask](https://flask.palletsprojects.com/en/2.1.x/tutorial/layout/).

With these tools all the tasks in developing projects are automated thereby saving time while making your work reusable by yourself and other developers.

**Directory Structure for a Data Science project**

*[from the Cookiecutter Data Science website](https://drivendata.github.io/cookiecutter-data-science/)*

```markdown
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- Make this project pip installable with `pip install -e`
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini 
```