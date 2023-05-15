# Introduction to Python

Instructor Vincent Beauregard






---

## Objectives

1. 👻 Read Python code and write it
2. 👬 Understand main differences between R and Python
3. 🧭 Orient yourself in the Python ecosystem for data science





---


🙋‍♂️🙋‍♀️ How have they heard from Python, why they want to use it (I want good and bad reasons)

---

## Why use Python

Python is popular 🏆

[Source : Stackoverflow survey 2022](https://survey.stackoverflow.co/2022/#technology-most-popular-technologies)

---

## Python fields of application
    1. Web development 💻
    2. Machine learning and AI 🧠
    3. Computer vision 👀
    4. Geographic Information System (GIS) 🌎
    5. Data science 🧪

[Awesome Python](https://awesome-python.com/#data-analysis)

---

## Python vs R for data science
### What's included
| 🔵base R | 🐍Python |
| ---
---
- | ---
---
- |
| * Data.frame<br />* `plot`<br /><br />*  `stats` | ¯\\\_(ツ)_/¯ |

---

## Python vs R for data science
### package ecosystem
|| 🔵R ecosystem | 🐍Python ecosystem|
| -- | ---- | ------- |
|Data frames|Built-in `data.frame`, `tibble`|`pandas.Dataframe`|
|Data manipulation|`dplyr`, `tidyr`|`pandas`|
|Math and statistics|Built-in `stats`|`numpy`, `scipy`|
|Plotting|Built-in `plot`, `ggplot2`|`matplotlib`, `seaborn`|
|Machine learning|`caret`, `mlr3`|`scikit-learn`|
|Geographic Information System (GIS)|`sf`, `raster`, `terra`|`geopandas`, `rasterio`, ...|
|Web development|`shiny`|`flask`, `django`|
|Web dashboards|`shiny`|`dash`|

Cheatsheet : [Python for R users](https://towardsdatascience.com/cheat-sheet-for-python-dataframe-r-dataframe-syntax-conversions-450f656b44ca)

---

## How is it similar and different from R

||🔵R|🐍Python|
|--------|--------|--------|
|**Purpose**|Statistical and general data analysis|General purpose|
|**Math functions**|All included|Arithmetic included, `math` built-in package|
|**Dataframes**|Built `Data.frame` type|No built-in type|
||Functionnal programming|Functionnal & object oriented|
||Interpreted language|Interpreted language|

---

## Running Python scripts vs R

File extension `script.R` vs `script.py`

Running scripts : Rstudio Console 🏆

---

## Running Python scripts vs R

 1. From terminal : Python interpreter ([see link for installation](https://www.python.org/downloads/)))
 ```python
 python.exe hello_world.py
 # R equivalent
 # R CMD BATCH script.R #👎
 # or
 # Rscript script.R 
 ```
 1. Integrated development environments (IDEs) ([VS Code](https://code.visualstudio.com/) and [PyCharm community](https://www.jetbrains.com/pycharm/download/#section=windows))

 2. Jupyter notebooks ([installation](https://jupyter.org/install)
???

Main IDEs functionalities : code completion, linting, debugging, git integration, variable explorer, testing, terminal, ...

```cmd
where python
```
```sh
which python
```

---

## Installing and using packages

### Installing packages

From terminal
```shell
# Install packages
pip install pandas
pip install numpy
pip install matplotlib
```

### Loading packages

From script or module or notebook
```python
# Import packages
import pandas as pd # R: library(dplyr)
from scipy import stats # R: library(stats)
import matplotlib.pyplot as plt # R: library(ggplot2)
```

---

## Installing and using packages

### Using packages

Within script or module or notebook
```python
# Using packages
plt.plot([1, 2, 3, 4]) # R: ggplot(data.frame(x = 1:4), aes(x)) + geom_line()
```

**🚨Important🚨** :
In Python 🐍 when importing packages, only the `module` object is imported. To access the functions, you need to use the `module.function` syntax.

In R 🔵 the `library` function imports the functions directly in the global environment. To access the functions, you only need to use the `function` syntax.