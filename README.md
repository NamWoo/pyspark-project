# DNDS 2nd Spark Project

Udacity Data Scientist Nanodegree 2nd Capstone Project

https://github.com/NamWoo/pyspark-project


## contents
1. results
2. install and import version
3. files
4. References, Licensing, Authors, Acknowledgements


## results

The highest score is LogisticRegression. f1(0.6), precision(0.375), and recall(0.4615) were all the highest.


|model|precision|recall|f1|
|:---:|:---:|:---:|:---:|
|**LogisticRegression**|0.5|0.125|0.2|
|GBTClassifier|0.5|0.375|0.42|
|LogisticRegression|0.6|0.375|0.46


## install and import version

* pyspark version 2.4.3

```
from pyspark.sql import SparkSession
from pyspark.sql.functions import avg, col, concat, desc, explode, lit, min, max, split, udf, isnull
from pyspark.sql.types import IntegerType
from pyspark.ml import Pipeline
from pyspark.ml.classification import LogisticRegression, RandomForestClassifier, GBTClassifier, DecisionTreeClassifier, NaiveBayes
from pyspark.ml.evaluation import MulticlassClassificationEvaluator
from pyspark.ml.feature import CountVectorizer, IDF, Normalizer, PCA, RegexTokenizer, StandardScaler, StopWordsRemover, StringIndexer, VectorAssembler
from pyspark.ml.regression import LinearRegression
from pyspark.ml.tuning import CrossValidator, ParamGridBuilder

from pyspark.ml.classification import LinearSVC
from pyspark.ml.evaluation import BinaryClassificationEvaluator

import re
import datetime
import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns
import pyspark
import pyspark.ml
```




## files

* mini_sparkify_event_data.json - starting data file containing the streaming music provider's user logs
* Sparkify.html/ipynb - notebook used for POC in Udacity Workspace







## References, Licensing, Authors, Acknowledgements


Data Scientist Nano Degree 2nd. Final Spark Project.

and ref [1](https://github.com/udacity), [2](https://www.slideshare.net/ssuser760eb4/pyspark-ch-06-ml)