---
title: "Pandas Tutorial"
description: "overview of how to install and use the pandas Python package for data analysis"
date: 2022-03-09T21:45:28-05:00
draft: false
tags: [tutorials, Python]
---

Welcome to this pandas tutorial, written by yours truly.

## Table of Contents

1. [About](#about)
2. [Features](#features)
3. [Obtaining the Resource](#obtaining-the-resource)
4. [Set Up](#setup)
5. [Execution](#execution)

### About

Describe the software resource and explain its relevance to your topic. Please include the link to the software resource.

The software resource I have decided to research is [pandas](https://pandas.pydata.org/), which is a tool for data analysis and manipulation, built using Python. This resource is relevant to my topic because it is a tool specifically for data analysis, which is my current career aspiration.

---

### Features

Outline the main features of the software. Why is this software necessary for your work?

The main features of this software include being able to read, write, and manipulate tabular data, while being able to calculate summary statistics and perform transformations of the data. This software is necessary for my work because it allows me to perform quick and easy transformations of large data sets, which will be useful for me, if I decide to work with analyzing large data sets for my comp.

---

### Obtaining the resource

Where do you find this software resource? Is it an open source project? an online tool? How do you install it? Are there any libraries that are also necessary to install?

This software resource can be found via its documentation [site](https://pandas.pydata.org/), but it can also be found on PyPI. This software resource is an open-source project and tool that can be installed in several ways, but the recommended installation method is through installing "as part of the Anaconda distribution, a cross platform distribution for data analysis and scientific computing". You can also install using pip from PyPI, ActivePython, Linux distribution's package manager, or through downloading the source code. While there did not appear to be any external libraries that needed to be installed, I found that NumPy is required to be installed before being able to use pandas. This is because pandas is built on top of the NumPy package, meaning both are needed to operate pandas.

---

### Setup

Include steps of all necessary steps to get the software to run (for example, installations). Include the commands to run if necessary.


- Step 1: Installation

Before starting installation, make sure that you have a working version of Python installed. (which I have installed)

Install pandas via your preferred method, mine is using pip to install using PyPI.

The command I'll use is: `pip install pandas`

Keeping in mind that I might also need NumPy, I'll use `pip install numpy`, to install that as well.

- Step 2: Set-Up

After running the pip install commands, you are ready to use pandas (and NumPy)! You start by setting up a standard Python program file.

**Example File Set Up**

```python
import pandas as pd

data = {
	'make':["Jeep", "Ford", "Nissan"],
	'model':["Wrangler", "Focus", "Altima", "Compass", "Fiesta", "Versa"],
	'year':[2000, 2010, 2020]
}

var = pd.DataFrame(data)

print(var)
```

The above example program creates a DataFrame using pandas and then prints it to the console in a 2D array structure, like a table.

In the next section, I will go more in depth in describing the functionality of pandas and provide some examples of its main functionality.

---

### Execution

How do you get the resource ready to use? Are there inputs to know? Please show a step-by-step guide (in a tutorial format) for readying the resource for your work. Include screenshots of successful execution and use of the software.

Luckily, there isn't much to do in terms of getting pandas ready for use, besides ensuring that *both* Python and pandas are installed before proceeding. That being said, in order to use pandas, you will need a general understanding of Python and how to write programs in Python.

There are a number of useful things that you are now able to do with data in Python once you import pandas as a module. You can create series, dataframes, read into CSV files, clean and analyze data, and construct correlations. I will be going through each of these functions, in its most basic construction, to provide an example for each.

- Series

In pandas, a *series* resembles a 1D array or a singular column in a table.

**Example**

```python
import pandas as pd

x = [1, 5, 9]

num = pd.Series(x)

print(num)
```

The expected output of the above program is:

```md
0	1
1	5
2	9
```

If you wanted to give your rows specific name assignments, instead of the default numerical values, you can use the index argument to customatize these values.

This would look somehting like:

```python
import pandas as pd

x = [1, 5, 9]

num = pd.Series(x, index = ["a", "b", "c"])

print(num)
```

The above should generate something like this:

```md
a	1
b	5
c	9
```

You can also construct Series from a dictionary. This looks like:

```python
import pandas as pd

age = {"Alexa": 21, "Jason": 9, "Mike": 35}

patients = pd.Series(age)

print(patient)
```

Using this approach allows you to construct a series that can either include all of the data points or only a select group, which can be modified using the index argument.

`patients = pd.Series(age, index = ["Alexa", "Mike"])`

This will print only the rows named Alexa or Mike, but not Jason.

- Data Frames and Reading into CSV files

In the previous section, I give a brief description and example of a DataFrame. Besides referencing that example, another helpful thing to know with DataFrames is how to load an exisiting CSV file into the DataFrame.

```python
import pandas as pd

data = pd.read_csv('data.csv')

print(data)
```

- Analyze Data

There are a handful of useful lines that can be used to analyze data using pandas.

To get an overview of the data set you are working with, you can print the first and the last 5 rows of your data set. This can be done like this:

`print(df.head())` in order to print the first 5 rows.

`print(df.tail())` in order to print the last 5 rows.

In order to get some more information from your data, you can use this line: `print(df.info())`

- Clean Data

There are a couple of ways that pandas supports cleaning data.

One way is by removing rows with empty cells, which can be done using a line like `data.dropna(inplace = True)`.

You can also replace the empty cells with new values, which can be done using a line like `data.fillna(10, inplace = True)`. This will replace all of the empty cells with the number 10.

If you want to only replace the empty cells of a specific column then use this line instead: `data["age"].fillna(10, inplace = True)`

You can also remove rows with null values in specific columns using a line like this: `data.dropna(subset=['age'], inplace=True)`

You can remove duplicate rows using the drop_duplicates() method like this: `data.drop_duplicates(inplace=True)`

- Correlations

You can check to see the relationships between the columns of your dataset easily, using a line like: `data.corr()`

Obviously, there are more things that are possible using pandas, but this is just a brief overview to get you started.

---

### Helpful resources

Include some of the relevant resources (links, articles, etc.) that you used to write in your tutorial.

	- [Official Documentation for Pandas](https://pandas.pydata.org/)
	- [Official Documentation for NumPy](https://numpy.org/install/)
	- [W3Schools Pandas Tutorial](https://www.w3schools.com/python/pandas)
