# Jupyter Presentation

Jupyter is a language agnostic notebook platform that works with a variety of different programming languages in a variety of different ways, including R, Julia, and Python!
This presentation utilizes seaborn/matplotlib and pandas for most of the data mangling, while R is used for the statistical analysis. 
The slidesshow feature of Jupyter along with the plugin RISE is used to create a dynamic presentation that is interleaved with the data analysis to create on-the-fly graphs.
 

## Instalation
1. Install Anaconda package manager https://www.anaconda.com/
2. Create an environment containing both Python3 and R
3. Install all dependencies (note: possible issues between the built in R package manager and Conda may come about, in such a case try defaulting to Conda packages)
4. Install RISE (https://github.com/damianavila/RISE) of interactive presentation capabilities.

## Using R magic cells on a python kernel. 
Inorder to use magic cells, get and install rpy2 (https://rpy2.readthedocs.i0)

To activate the R magic in Jupyter, execute these commands in python cell:
```
%matplotlib inline
%load_ext rpy2.ipython
```


## Dependencies

R Dependencies
```
library(MASS)  # for boxcox
library(reshape2)
library(dplyr)
library(tidyr)
library(ez)
library(knitr)
library(ggplot2)
library(ARTool)
library(gmodels) # for ci
library(car)
library(lsmeans)
```

Python Dependencies
``` 
import json
import os
import csv
import re

import math
import numpy as np
import pandas as pd
import statsmodels.formula.api as smf       # for ANOVA
import statsmodels.stats.multicomp as multi # for post hoc test 
import statsmodels.api as sm
from sklearn import linear_model
from sklearn import preprocessing
from sklearn.preprocessing import normalize
import scipy.spatial.distance as distance
import scipy.stats as stats
from scipy.stats import boxcox
from scipy.stats import skew
from pyquaternion import Quaternion
from matplotlib.backends.backend_pdf import PdfPages

from scipy import stats, integrate
import matplotlib.pyplot as plt
import matplotlib

import seaborn as sns
import math
import sys
import subprocess

# Import analysis Scripts
import nbimporter
import Analysis_Util as analysis_util
```

