---
permalink: /files/
title: "Anaconda Tips"
author_profile: true
redirect_from: 
  - /md/
  - /anaconda.html
---

## Installing Anaconda
Please follow the instruction [here](https://docs.anaconda.com/anaconda/install/windows/) for installing Anaconda on your OS

## Anaconda Commands
First run Anaconda Prompt

| C:\Users\user>set "JAVA_HOME_CONDA_BACKUP="   C:\Users\user>set "JAVA_HOME=C:\Users\user\Anaconda3\Library"                                                       (base) C:\Users\user> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## Installing R and RStudio

- First, run ```conda install -r essentials``` on Anaconda Prompt.
- then, run ```conda install -c r rstudio``` on Anaconda Prompt.


## Installing and updating packages

- To list all of the packages in the active environment, use: ```conda list``` on Anaconda Prompt
- To update a package, use ```python -m pip install -U package```. For example, to update *matplotlib* we can use ```python -m pip install -U matplotlib```
