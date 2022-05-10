---
title: "Experiment"
description: "a summary of my experiment and its results"
date: 2022-05-09T22:26:42-04:00
draft: true
tags: [data-analysis, R]
---

##### Summary of experiment

My experiment takes the data set that my prototype was based on, [California Educational Attainment and Personal Income](https://data.ca.gov/dataset/ca-educational-attainment-personal-income), and expands upon the analysis that was performed for 2008 data in my prototype. My intention in creating my prototype was to look into how poverty effects educational attainment and/or access to education. The main goal of my experiment is to answer the question of how educational attainment for those below the poverty line changed between the 2008 and 2010. I also separate my analysis by gender to see differences in rates of educational attainment and the differences in the amount of people experiencing poverty between both genders.

The first thing I had to do to complete my experiment is revise my prototype. After completing my initial prototype submission, I found that I had discovered some tweaks I wanted to make in the current code in order to make the visualizations more concise and specifically wanted to look to combine the legends of the combined plots I made and add separate titles to the plots. Next, I will need to wrangle the 2010 data, like I did the 2008 data, because my intention is to study how poverty levels, educational attainment, and income levels changed between both years for people in California. Next I will need to create visualizations of 2010 data, similar to what I did for the 2008 graphs, and will then create comparative visualizations of the 2008 and 2010 data to further show the differences between both years. The last step in my experiment is to take the results from the visualizations and make some conclusions about the population at the time and how the different population, poverty, and educational metrics changed for them between 2008 and 2010.

##### Results

The results of my experiment are as follows:

**2008**

Considering the population of California is 36.54 million in 2008, we can make the following conclusions about the population at the time.

Highest female value is 740,143 (no hs diploma., no income) -- 2% of the population

*Considerations*

- Could be married and dependent on spouse's income
- Could be single and dependent on family's income

---

Highest male value is 573,769 (no hs diploma, 15k-24,999)  -- 1.6% of the population

*Considerations*

- Could indicate more high-school aged AND/OR older males are inclined/expected to work, contributing to the high count

---

**Conclusions for 2008**

- Female graph accounts for 5,434,192 ppl -- 14.9% of the population
- Male graph accounts for 4,057,275 ppl -- 11.1% of the population
- Total: 9,491.467 ppl under the poverty line - 25.98% of the population (1/4!)
- More women live under the poverty line than men in CA
- More women have no income and no high school diploma
- The findings have fewer men in the sample, which could indicate that most men live above the poverty line

**2010**

Considering the population of California is 37.27 million in 2010, we can make the following conclusions about the population at the time.

Highest female value is 666,858 ppl (no hs diploma, no income) - 1.8% of the pop.

*Considerations*

- Could be married and dependent on spouse's income
- Could be single and dependent on family's income

---

Highest male value is 535,027 ppl, (no hs diploma, 15k-24,999) -1.4% of the pop.

*Considerations*

- Could indicate more high-school aged AND/OR older males are inclined/expected to work, contributing to the high count

---

**Conclusions for 2010**

- Female graph accounts for 5,575,978 ppl - 14.96% of the pop
    - 897,367 ppl have a bachelor's degree or higher
	- 1,461,702 ppl have hs or equiv. education
	- 1,444,492 ppl have no hs diploma
	- 1,772,417 ppl have some college, less than 4yr degree
- Male graph accounts for 4,377,997 - 11.75% of the pop
	- bachelor's degree or higher: 550,304 ppl
	- hs or equiv. education: 1,279,104 ppl
	- no hs diploma: 1,426,338 ppl
	- some college, less than 4yr degree: 1,122,251 ppl
- 9,953,975 people live under the poverty line, 26.7% of the population
	- 462,508 more ppl than in 2008
- More women live under the poverty line than men in CA
- More women have no income and no high school diploma

**2008 v 2010**

*General Conclusion(s)*:

- Populations: 36.54 million (2008) | 37.27 million (2010) 
    - Population rose by 730,000 between 2008 and 2010.

*Female*

**Conclusions**

- In 2008 the highest female value was 740,143 (no hs diploma, no income), which accounted for about 2% of the population
- In 2010 the highest female value was 666,858 ppl (no hs diploma, no income), which accounted for about 1.8% of the population.
	- There were 73,285 fewer women with no income and no hs diploma in 2010 than in 2008 -- more women had a hs diploma and/or received an income in 2010 than in 2008.
- The female graph for 2008 accounts for 5,434,192 ppl, which is about 14.9% of the population.
- The female graph for 2010 accounts for 5,575,978 ppl, which is 14.96% of the population.
	- There were 141,786 fewer women under the poverty line in 2010 than in 2008.
- Educational Attainment Comparisons:
    - bachelor's degree or higher
        - 2008: 850,768
        - 2010: 897,367 ppl
	        - There are 46,599 more women below the poverty line with bachelor's degrees or higher in 2010 than in 2008.
    - high school or equivalent education
        - 2008: 1,432,888 
        - 2010: 1,461,702
	        - 28,814 more women have hs or equivalent education in 2008 than in 2010.
    - no hs diploma
        - 2008: 1,539,416
        - 2010: 1,444,492
	        - There are 94,924 fewer women that have no hs diploma in 2010 than in 2008.
    - some college, less than 4yr degree
        - 2008: 1,611,120
        - 2010: 1,772,417
	        - There are 161,297 more women that have completed some college in 2010 than in 2008.

---
*Male*

**Conclusions**

- In 2008, the highest male value is 573,769 (no hs diploma, 15k-24,999), which was 1.6% of the population at the time.
- In 2010, the highest male value is 535,027 ppl, (no hs diploma, 15k-24,999), which was 1.4% of the population.
	- There were 38,742 men who either have started earning different incomes or earning high school diplomas, or getting out of the "poverty line"
- The 2008 Male graph accounts for 4,057,275 ppl, which is 11.1% of the population
- The 2010 Male graph accounts for 4,377,997, which is 11.75% of the pop
	- There were 320,722 more men that feel below the poverty line between 2008 and 2010
- Educational Attainment Comparisons:
    - bachelor's degree or higher
	    - 2008: 436,046
        - 2010: 550,304
	        - 114,258 more men received a bachelor's degree in 2010 than in 2008
    - high school or equivalent education
        - 2008: 1,215,408
        - 2010: 1,279,104
        	- There were 63,696 more men who received a hs or equiv education
    - no hs diploma
        - 2008: 1,315,323
        - 2010: 1,426,338
	        - There were 111,015 more men who had no hs diploma
    - some college, less than 4yr degree
        - 2008: 1,090,498
        - 2010: 1,122,251 ppl
	        - There were 31,753 more men who had some college and less than a 4 yr degree
