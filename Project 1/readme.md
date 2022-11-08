# Welcome to Project 1: Bayesian Structure Learning 

After finishing this project, you will be able to get thorough understanding about Bayesian Network and Structure Learning.

![alt text](https://github.com/bonaldli/DMU-Uni-Koeln/blob/main/Project%201/intro.png?raw=true)

## Datasets
First of all, we have three datasets, and the summaries are given as below:
| Dataset  | Number of Variables | Source | Further Reading | Content |
| ------------- | ------------------- | ------------- | -------------------------------------- | ------------- |
| Titanic Data | 8 | [Kaggle](https://www.kaggle.com/c/titanic) | (1) [probability](https://web.stanford.edu/class/archive/cs/cs109/cs109.1166/problem12.html) | (1) original data; (2) simplified data (recommended)|
| Wine Prediction Data | 12 | [Kaggle](https://www.kaggle.com/datasets/dropout/winequalityred) |  (1) [descriptive analysis](https://rpubs.com/Hpolhe/950288) (in R); (2) [sales prediction case](https://rstudio-pubs-static.s3.amazonaws.com/840867_cdbf78a38ded4b10be5af93271ee7593.html#DATA_EXPLORATION)| (1) original data; (2) simplified data (recommended) |
| California House Price (Bonus) | 10 | [Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices) | (1) [descriptive analysis](https://inria.github.io/scikit-learn-mooc/python_scripts/datasets_california_housing.html) | try original data |

## Task
You will use python to learn the structure for the datasets of _Titanic_ and _Wine_, associated with the Bayesian Score. The input and output are required as follows. You could take a look at the example.
- **Input:** `example.csv` (using the simplified data is recommended)
- **Output:** `example.gph`, `example.pdf`, `example.score`
- A specific example of a graph for Titanic dataset with only 3 edges (numsiblings ➝ numparentschildren, numsiblings ➝ passengerclass, numparentschildren ➝ sex) will look like `titanicexample.gph`.

## Hint:
- Python is recommended. However, you could use any programming language that you prefer. 
- If you use packages that is directly related to Bayesian structure learning, then you are recommended to write down the functions from the packages on your own way. 
- The Python package for optimization are recommended for your to use:
  - `NetworkX`
  - `bnlearn`
- Discussions are encouraged.

## Example:
You could find the examples in the `Example` folder. And most importantly, you could follow the tutorial [here](https://github.com/bonaldli/DMU-Uni-Koeln/blob/main/Project%201/Example/A%20Step-by-Step%20Guide%20in%20detecting%20causal%20relationships%20using%20Bayesian%20Structure%20Learning%20in%20Python.pdf).

## Grading:
- Titanic Graph (`titanic.gph`): 20%
- Wine Graph (`wine.gph`): 30%
- Report: 50%
  - Description of algorithm: 10%
  - Visualization of output graphs: 10%
  - Code (in PDF): 10%
  - Interpretation and analysis of the results: 10%
  - Reference: 10%
- Bonus:
  - California Graph (`california.gph`): + 20%
  - Report: + 30%
    - Description of algorithm: 10%
    - Visualization of output graphs: 10%
    - Code (in PDF): 10%

## Template
Please use the given Overleaf [Template](https://www.overleaf.com/read/fqpyqzzjvfzy) for writing for project report.

## Submission
Send me your `.zip` file to my email before the deadline: **23:59 PM, 20 Nov 2022** (updated). The file should includes following:
- `.gph` files (x2 or x3): `titanic.gph`, `wine.gph`, (`california.gph`)
- `.pdf` file (x1): `Project 1 Report-First Name-Last Name.pdf`
