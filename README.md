# Workbooks for Big Data and Social Science

**Brian Kim, Christoph Kern, Jonathan Scott Morgan, Clayton Hunter, Avishek Kumar**

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master)

Notebook Descriptions and Links
------------

## Databases

[Link to Databases notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=01_Databases.ipynb)


The *Databases* notebook builds the foundation of using SQL to query data. 
Much of the later notebooks will involve using these tools. This workbook 
also introduces you to the main data source that is used in the online workbooks, 
the North Carolina Department of Corrections Data 
(<https://webapps.doc.state.nc.us/opi/downloads.do?method=view>). In this notebook, you will:

- Build basic queries using SQL,

- Understand and perform various joins. 

## Dataset Exploration and Visualization

[Link to Dataset Exploration and Visualization notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=02_Dataset_Exploration_and_Visualization.ipynb)

The *Dataset Exploration and Visualization* notebook further explores the 
North Carolina Department of Correction data, demonstrating how to work with 
missing values and date variables and join tables by using SQL in Python. 
Though some of the SQL from the Databases notebook is revisited here, the 
focus is on practicing Python code and using Python for data analysis. The 
workbook also explains how to pull data from a database into a dataframe 
in Python and continues by exploring the imported data using the `numpy` 
and `pandas` packages, as well as `matplotlib` and `seaborn` for 
visualizations. In this workbook, you will learn how to:

- Connect to and query a database through Python,

- Explore aggregate statistics in Python,

- Create basic visualizations in Python.

## APIs 


[Link to APIs notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=03_API.ipynb)

The *APIs* notebook introduces you to the use of Internet-based web service 
APIs for retrieving data from online data stores. This notebook walks through 
the process of retrieving data about patents from the PatentsView API from 
the United States Patent and Trademark Office. The data consist of information 
about patents, inventors, companies, and geographic locations since 1976. 
In this workbook, you will learn how to:

-   Construct a URL query,

-   Get a response from the URL,

-   Retrieve the data in JSON form.

## Record Linkage

[Link to Record Linkage notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=04_Record_Linkage.ipynb)

In the *Record Linkage* workbook, you will use Python to implement the basic
concepts behind record linkage using data from PatentsView and Federal 
RePORTER. This workbook will cover how to pre-process data for linkage before demonstrating multiple methods of record linkage, including probabilistic record linkage, 
in which different types of string comparators are used to compare multiple 
pieces of information between two records to produce a score that indicates 
how likely it is that the records are data about the same underlying entity. 
In this workbook, you will learn how to:

-   Prepare data for record linkage,

-   Use and evaluate the results of common computational string
    comparison algorithms including Levenshtein
    distance, Levenshtein--Damerau distance, and Jaro--Winkler distance,

-   Understand the Fellegi--Sunter probabilistic record linkage method,
    with step-by-step implementation guide.

## Text Analysis 

[Link to Text Analysis notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=05_Text_Analysis.ipynb)

In the *Text Analysis* notebook, you will use the data that you pulled from 
the PatentsView API in the API notebook to find topics from patent abstracts. 
This will involve going through every step of the process, from extracting 
the data to cleaning and preparing to using topic modeling algorithms. 
In this workbook, you will learn how to:

- Clean and prepare text data,

- Apply Latent Dirichlet Allocation for topic modeling,

- Improve and iterate models to focus in on identified topics.

## Networks

[Link to Networks notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=06_Networks.ipynb)

In the *Networks* workbook you will create network data where the nodes
are researchers who have been awarded grants, and ties are created
between each researcher on a given grant. You will use Python to read
the grant data and translate them into network data, calculate node- 
and graph-level network statistics and create network visualizations. 
In this workbook, you will learn how to:

-   Calculate node- and graph-level network statistics,

-   Create graph visualizations. 

## Machine Learning -- Creating Labels

[Link to Machine Learning notebook 1](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=
07_1_Machine_Learning_Labels.ipynb)


The *Machine Learning Creating Labels* workbook is the first of a three-part Machine Learning workbook sequence, starting with how to create an 
outcome variable (label) for a machine learning task by using SQL in Python. 
It uses the North Carolina Department of Corrections Data to build an 
outcome that measures recidivism, i.e. whether a former inmate returns to 
jail in a given period of time. It also shows how to define a Python 
function to automate programming tasks. In this workbook, you will learn 
how to:

-   Define and compute a prediction target in the machine learning framework,

-   Use SQL with data that has a temporal structure (multiple records per observation).

## Machine Learning -- Creating Features

[Link to Machine Learning notebook 2](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=07_2_Machine_Learning_Features.ipynb)

The *Machine Learning Creating Features* workbook prepares predictors 
(features) for the machine learning task that has been introduced in the 
*Machine Learning Creating Labels* workbook. It shows how to use SQL 
in Python for generating features that are expected to predict recidivism,
such as the number of times someone has been admitted to prison prior to 
a given date. In this workbook, you will learn how to:

-   Generate features with SQL for a given prediction problem,

-   Automate SQL tasks by defining Python functions.

## Machine Learning -- Model Training and Evaluation

[Link to Machine Learning notebook 3](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=07_3_Machine_Learning_Models.ipynb)

The *Machine Learning Model Training and Evaluation* workbook uses the 
label and features that were created in the previous workbooks to construct 
a training and test set for model building and evaluation. It walks through examples on 
how to train machine learning models using `scikit-learn` in Python and how 
to evaluate prediction performance for classification tasks. In addition, 
it demonstrates how to construct and compare many different machine learning models in Python. In this workbook, you will learn how to:

-   Pre-process data to provide valid inputs for machine learning models,  

-   Properly divide data with a temporal structure into training and test sets,

-   Train and evaluate machine learning models for classification using Python.

## Bias and Fairness

[Link to Bias and Fairness notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=08_Bias_and_Fairness.ipynb)


The *Bias and Fairness* workbook demonstrates an example of using the bias and 
fairness audit toolkit Aequitas in Python. This workbook uses an example 
from criminal justice and demonstrates how Aequitas can be used to 
detect and evaluate biases of a machine learning system in relation to 
multiple (protected) subgroups. You will learn how to: 

- Calculate confusion matrices for subgroups and visualize performance metrics by groups,

- Measure disparities by comparing, e.g., false positive rates between groups,

- Assess model fairness based on various disparity metrics.

### Errors and Inference

[Link to Errors and Inference notebook](https://mybinder.org/v2/gh/Coleridge-Initiative/bdss-notebooks/master?filepath=09_Errors_and_Inference.ipynb)

The *Errors and Inference* workbook walks through how one might think critically about issues that might arise in their analysis. In this notebook, you will evaluate the machine learning models from previous notebooks and learn about ways to improve the data to use as much information as possible to make conclusions. Specifically, you will learn how to: 

- Perform sensitivity analysis with machine learning models,

- Use imputation to fill in missing values.
