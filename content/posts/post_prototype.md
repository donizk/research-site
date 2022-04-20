---
title: "Prototype"
description: "a description of my senior comp prototype"
date: 2022-04-20T14:59:50-04:00
draft: false
tags: [data-analysis]
---

### Brief description of my prototype

The main goal I had in mind when developing my prototype deliverable is to create a tool that will automatically harvest data and download it to be used in R-Studio. This tool employs R and R-Studio, which will both be needed to run the tool.

Currently, the main functionality of the tool is to:

- take a given URL to harvest the data from
- download dataset to local machine
- wrangle dataset to relevant variables
- create visualizations from dataset

The dataset being used for this tool is the [California Educational Attainment and Personal Income](https://data.ca.gov/dataset/ca-educational-attainment-personal-income), which is data captured by the U.S. Census Current Population Survey (CPS). The dataset includes information on the year the data is captured, the age and gender of the person being surveyed, the level of educational attainment, personal income of the respondent, and the number of people who fall into the same category (given the prior values). I chose this dataset as it was the closest to the variables I wanted to analyze, education and income, and was more easily processed by my machine over alternative datasets I had been looking at. The tool can be run by opening the file that hosts the code, prototype-code.R, on R-Studio and going line by line to run the commands.
