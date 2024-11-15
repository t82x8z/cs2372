java c
CIV 1320 Indoor Air Quality
Homework Assignment 2

September 18, 2024
DUE: October 9, 2024 9 am
55 pts total
1. Mass Balance - ETS  10 pts
Cigarette smoking produces a wide variety of compounds that are known as environmental t   obacco smoke (ETS). The average emissions of particulate matter (PM2.5) from cigarettes are 13.7 mg/cigarette. The purpose of this problem is to predict the levels of PM2.5  that result from smoking a single cigarette for 10 minutes in a small apartment (50 m3).  The only removal mechanisms of particles are dilution by means of 30 m3/h of natural infiltration and deposition to surface with a loss rate of 0.1/h.  There are no other sources of particulate matter inside or outdoors.
a)Derive and solve the governing equations for PM2.5  concentration as a function of time in the apartment.
b)Plot your results in the form. of concentration vs. time with the x-axis extending for 3 hours from the end of the smoking episode.
c)If the smoker smokes one cigarette each 30 minutes, what will the concentration be after 3 hours in the space?
d) Repeat a) and b) using a portable air cleaner with a CADR of 100 m3/h.  What is the mean effectiveness of the air cleaner while the smoking is occurring?
2. Ozone generation indoors  15 pts
This question uses data that is in a file hw2 2 data.xls.
You are interested in determining the emission rate of an air “cleaner” that generates ozone. To measure the ozone emission rate, E (mg/h), you put the air cleaner in 20 m3 chamber and turn it on. For the entire experiment, the air exchange rate (Q/V) for the chamber is 0.5/h (all with a dedicated ozone free air supply). After it has run for 70 minutes, you turn the air cleaner off and continue to measure the ozone concentration in the chamber for 20 more minutes. Using the data in the file, answer the following questions.
a) What is the ozone emission rate (mg/h) for the air cleaner?
Hint: Calculate the deposition loss rate from the last 20 minutes of the data, and use this value in the analysis of the first portion of the data set.
b) Is the ozone concentration in the chamber at steady state at t = 70 minutes?  If you assume steady state at t = 70 min, what is the emission rate (mg/h).  Does the ozone concentration need to be at steady state for your answer in part a) to be valid?  Justify your answers.
3. Comparing portable and centralized air cleaning                                                          30 pts
You are faced with the task of making a recommendation about whether to use portable air cleaners or ordinary HVAC filters in residential environments for PM2.5.  The data about relevant homes and air cleaners is in the table on the next page.
a)  Derive a time-averaged equation for effectiveness for both portable air cleaner (assuming that it runs constantly) and HVAC filtration.  What assumptions are you making with these equations?  Are they reasonable?  Are they equally reasonable for both types of air cleaning?
b)  Using the data in the table above generate a Monte Carlo model for both effectiveness equations.  You will need to use software to do this.  The following instructions are for Excel, but many other software packages can do this (and do so even better…).  Excel has two ways of generating random numbers the rand() function which generates a random number between 0 and  1 and randbetween(lower,higher) w代 写CIV 1320 Indoor Air Quality Homework Assignment 2
代做程序编程语言hich generates a random integer between lower and higher.   Note that all random numbers change every time a worksheet is recalculated.  There are ways of turning this on and off that are detailed in the help file for Excel.  The trick is going from a uniformly distributed random number to a different statistical distribution.  For uniform. distributions of continuous variables you can just scale the rand() function by doing rand()*(higher-lower)+lower where higher and lower are the higher and lower value of the ranges.  For other statistical distributions you  can use functions such as norminv and loginv which take a probability from 0 to 1 and convert to a value from a distribution with known parameters, so, for example norminv(rand(), mean, standard deviation) will generate a random value from the normally distributed variable that has a mean value of mean and a standard deviation of standard deviation.  One quick clarification on the lognormal functions in Excel is that they typically expect log-transformed parameters so you have to use the arguments ln(GM) and ln(GSD) rather than the actual values.  Also, some values could theoretically be not physically realistic based on the statistical distribution and so they have minimum  values that you can address with an if function.
Variable
Distribution
Parameters
Air exchange rate, λ
Lognormal
Murray  Burmaster (1995), all homes
Deposition loss rate, β
Normal
Williams et al. (2003), k
Portable CADR
Uniform
50 – 500 m3/h
Floor area
Normal
µ = 200 m2, σ = 60 m2, min 50 m2
Ceiling height
Fixed
2.5 m
Run time fraction
Uniform
5-20%, uniform
HVAC Filter efficiency
Uniform
30-70%, uniform
Recirculation rate
Normal
µ = 4/h , σ = 1/h, min 0.5/h
c)   Try copying your effectiveness calculations for 100 cells (or 100 loops of an iterative
approach) and seeing if the median effectiveness changes by more than 1 percentage point with each recalculation. If so, try 500 cells, then 1000 cells, then 5000 cells, then 10000 cells. If easy, keep going until you meet the 1% criterion (if you haven’t already met it).   How many iterations would you recommend to meet this criterion?  Why does the median make sense to use as an averaging statistic, rather than the mean?
d)  Which air cleaning strategy is more effective?  By what amount?
e)   If you want a strategy that has an 80% or better effectiveness in half of the homes, how much would you have to increase CADR (to make it easier, keep the relative range of higher/lower = 10 as in the original problem)?  Is this practical?  Can you achieve this same performance by improving filter efficiency?  If not how much do you have to increase the recirculation rate (assuming 100% runtime) with the same filter to achieve this performance metric?  Is this feasible?  Which approach (portable or central) would you recommend for a national strategy?
f)   How sensitive is your answer d) to the following changes?
a.   If b = 0.01 (fixed), CADR and filter efficiency stays approximately the same (for example, smaller particles).
b.   If b = 1 (fixed), CADR stays the same, and filter efficiency increases to 80-100% (for example, larger particles).
g)  What would you do if you had an important variable with no knowledge of the distribution? How could you integrate it into this model?

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
