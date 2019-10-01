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


## Installing R and RStudio

- First, run ```conda install -r essentials``` on Anaconda Prompt.
- then, run ```conda install -c r rstudio``` on Anaconda Prompt.


## Installing and updating packages

- To list all of the packages in the active environment, use: ```conda list``` on Anaconda Prompt
- To update a package, use ```python -m pip install -U package```. For example, to update *matplotlib* we can use \n
```python -m pip install -U matplotlib```
