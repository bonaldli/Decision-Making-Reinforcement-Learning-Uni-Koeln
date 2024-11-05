# Welcome to Project 1: Bayesian Structure Learning 

After finishing this project, you will have a thorough understanding of Bayesian Network and Structure Learning.

![alt text](https://github.com/bonaldli/DMU-Uni-Koeln/blob/main/Project%201/intro.png?raw=true)

## Datasets
First of all, we have three datasets, and the summaries are given as below:
| Dataset  | Number of Variables | Source | Further Reading | Content |
| ------------- | ------------------- | ------------- | -------------------------------------- | ------------- |
| Titanic Data | 8 | [Kaggle](https://www.kaggle.com/c/titanic) | (1) [probability](https://web.stanford.edu/class/archive/cs/cs109/cs109.1166/problem12.html) | (1) original data; (2) simplified data (recommended)|
| Wine Prediction Data | 12 | [Kaggle](https://www.kaggle.com/datasets/dropout/winequalityred) |  (1) [descriptive analysis](https://rpubs.com/Hpolhe/950288) (in R); (2) [sales prediction case](https://rstudio-pubs-static.s3.amazonaws.com/840867_cdbf78a38ded4b10be5af93271ee7593.html#DATA_EXPLORATION)| (1) original data; (2) simplified data (recommended) |
| California House Price (Bonus) | 10 | [Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices) | (1) [descriptive analysis](https://inria.github.io/scikit-learn-mooc/python_scripts/datasets_california_housing.html) | try original data |

## Task
You will use Python to learn the structure for the datasets of _Titanic_ and _Wine_, associated with the Bayesian Score. The input and output are required as follows. You could take a look at the example.
- **Input:** `example.csv` (using the simplified data is recommended)
- **Output:** `example.gph`, `example.pdf`, `example.score`
- A specific example of a graph for Titanic dataset with only 3 edges (numsiblings ➝ numparentschildren, numsiblings ➝ passengerclass, numparentschildren ➝ sex) will look like `titanicexample.gph`.

## Hint:
- Python is recommended. However, you could use any programming language that you prefer.
- There are two tracks of solutions you can use: (1) simple heuristic algorithms from textbook (K2, Local Search, Genetic), or (2) solution from the paper NoTears
  - If you choose Track 1:
    - Please try your best not to directly use the structure learning package in Python (for example: directly use the package of `NetworkX' and `bnlearn', and directly get your graph); instead, try to write down your own code (for example, write down your own `score' function, your own `searching' function) based on whatever algorithm you wanna use.
    - But, you can of course refer to theses packages, see what's their function, how is it achived in code, then you are recommended to write down the functions from the packages in your own way. And your code should be runnable as-is: direct input and can get the output.
  - If you choose Track 2:
    - You can directly use the code that is available in github for NoTear, and try to reproduce the result first.
    - You should also discuss how you determine the L1-penalty tuning parameter, and how it affects your result.
- In the Bonus, if you don't like the California Dataset, you could find your own dataset. And in your report, briefly introduce your own dataset.
- Discussions are encouraged.

## Example:
You can find the examples in the `Example` folder. And most importantly, you could follow the tutorial [here](https://github.com/bonaldli/DMU-Uni-Koeln/blob/main/Project%201/Example/A%20Step-by-Step%20Guide%20in%20detecting%20causal%20relationships%20using%20Bayesian%20Structure%20Learning%20in%20Python.pdf).

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
Submit your `.zip` file to the ILIAS system before the deadline: **23:59 PM, 26 Nov 2023** (updated). The file should includes following:
- `.gph` files (x2 or x3): `titanic.gph`, `wine.gph`, (`california.gph`)
- `.pdf` file (x1): `Project 1 Report-First Name-Last Name.pdf`
