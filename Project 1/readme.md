# Welcome to Project 1: Bayesian Structure Learning 
After finishing this project, you will be able to get thorough understanding about Bayesian Network and Structure Learning.

## Datasets
First of all, we have three datasets, and the summaries are given as below:
| Dataset  | Number of Variables | Source | Further Reading | Content |
| ------------- | ------------------- | ------------- | -------------------------------------- | ------------- |
| Titanic Data | 8 | [Kaggle](https://www.kaggle.com/c/titanic) | (1) [probability](https://web.stanford.edu/class/archive/cs/cs109/cs109.1166/problem12.html) | (1) original data; (2) simplified data (recommended)|
| Wine Prediction Data | 12 | [Kaggle](https://www.kaggle.com/datasets/dropout/winequalityred) |  (1) [descriptive analysis](https://rpubs.com/Hpolhe/950288) (in R); (2) [sales prediction case](https://rstudio-pubs-static.s3.amazonaws.com/840867_cdbf78a38ded4b10be5af93271ee7593.html#DATA_EXPLORATION)| (1) original data; (2) simplified data (recommended) |
| California House Price (Bonus) | 10 | [Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices) | N/A | try original data |

## Task
You will use python to learn the structure for the datasets of _Titanic_ and _Wine_, associated with the Bayesian Score. The input and output are required as follows. You could take a look at the example.
- **Input:**: `example.csv`
- **Output:** `example.gph`, `example.pdf`, `example.score`
- A specific example of a graph for Titanic dataset with only 3 edges (numsiblings ➝ numparentschildren, numsiblings ➝ passengerclass, numparentschildren ➝ sex) will look like `titanicexample.gph`.

## Hint:
- Python is recommended. However, you could use any programming language that you prefer. 
- You are not recommended to use packages uploaded in the internet that is directly related to Bayesian structure learning.
- The Python package for optimization are recommended for your to use:
  - `NetworkX`
- Discussions are encouraged.

## Grading:
- Titanic Graph (`titanic.gph`): 20%
- Wine Graph (`wine.gph`): 30%
- Report: 50%
  - Overleaf [Template](https://www.overleaf.com/read/fqpyqzzjvfzy)
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
