# Simulation of PGA Tour Golf Data

## Programming for Data Analysis Project

### Andrew Walker - G00398788@gmit.ie

![www.pgatour.com](https://pga-tour-res.cloudinary.com/image/upload/c_fill,dpr_2.6,f_auto,g_center,h_336,q_auto,w_1320/v1/pgatour/editorial/2020/12/17/Logo/flag-example-1400.jpg)

## 1. Introduction

This repository contains a Jupyter notebook and files containing data related to the notebook demonstrating my work on the Programming for Data Analysis Project. The project instructions required students to create a data set by simulating a real-world phenomenon of their choosing. Then, students should model and synthesise such data using Python.

Specifically, the project instructions were as follows:

- Choose a real-world phenomenon that can be measured and at least one-hundred data points across at least four different variables can be collected.

- Investigate the types of variables involved, their likely distributions, and their relationships with each other.

- Synthesise/simulate a data set as closely matching their properties as possible.

- Detail the research and implement the simulation in a Jupyter notebook – the data set itself can simply be displayed in an output cell within the notebook.

The instructions suggested that the `numpy.random` package was used to simulate data but, following research and experimentation, the `scipy.stats` module was considered to provide better functionality for the simulation task and was used instead. 

## Project Description

The project simulates a data set based on historical PGA Tour golf statistics and models the relationships between four variables:

- Driving distance average (the average number of yards per hole)

- Driving accurary percentage (the percentage of time a tee shot comes to rest in the fairway)

- Greens in Regulation (GIR) percentage (the percent of time a player was able to hit the green in regulation. The GIR stroke is determined by subtracting 2 from par)

- Birdie average (the average number of birdies made per round played.)

The [R&A and USGA Distance Insights Report (2020)](https://www.usga.org/content/dam/usga/pdf/2020/distance-insights/DIPR-FINAL-2020-usga.pdf) finds that the average driving distance on the PGA Tour has shown a general increase, in particular from the early 1990s with the introduction of oversized drivers. Following this, further technological and rule innovations has led to a trend in increased distance off the tee. However, the Distance Insights Report (2020) also finds that as driving distance increases, driving accuracy decreases.

The project makes a comparison of the above four variables to:

1. Model how driving distance affects accuracy
2. Model how distance and accuracy affect the number of greens in regulation hit
3. Model how distance and accuracy affect the number of birdies scored
4. Model how the number of greens in regulation hit affects birdies

The project is described in further detail in the notebook itself.

 It is considered that it might be a useful simulation for golfers to establish if distance could be considered to be more important than accuracy, or vice versa, in the context of reaching in the green in fewer shots and scoring birdies.

## Install

Python distributions contain commonly used packages and tools. [Anaconda](https://www.anaconda.com/download/) works on Windows, Mac, and Linux, provides a large collection of packages. 

The notebook uses the following packages, which, if not installed on the user's computer might result in the notebook not functioning as intended:

- `pandas`
- `numpy`
- `matplotlib.pyplot`
- `seaborn`
- `fitter`
- `statistics`
- `scipy`

 If required, Python comes with an inbuilt package management system, [pip](https://pip.pypa.io/en/stable) which can install, update, or delete any official package (https://scipy.org/install/).

For example, to install `fitter`:

`pip install fitter` 

Further details are available on the [fitter website](https://pypi.org/project/fitter/).

Once installed, the packages must be imported; the notebook includes the necessary code to import all packages, once installed (if installation is required).

In addition to the above packages, the project contains several .csv files containing the Fedex Cup 2021 and historical PGA Tour data. These files are as follows and are contained in a separate `data` folder:

- strokes_gained.csv
- historic_accuracy.csv
- historic_birdies.csv
- historic_distance.csv
- historic_gir.csv

## Run

Users can view the notebook in static form by clicking the following badge: [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/AndyWalker81/ProgrammingForDataAnalysis_Project/blob/main/Programming_Project.ipynb)

Users can view the notebook in dynamic form by clicking the following badge: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AndyWalker81/ProgrammingForDataAnalysis_Project/HEAD?labpath=Programming_Project.ipynb)



## Explore

First, the notebook contains an introduction and details on required installations.

A set of data taken from the [PGA Tour website](https://www.pgatour.com/) consisting of the top 100 players by 2021 Fedex Cup rank is then presented. The name and data for each of the four variable is included. From these data, the `fitter` function determines the best-fit distribution for each variable. 

Next, data for each of the top 100 players within each variable category was collected from the PGA Tour website for the years 1990, 2000, 2010, and 2020. For each variable, the mean for each year is calculated. The increase or decrease between the mean value for each year is then determined - this gives an indication of whether, PGA Tour golfers, on average, have improved or worsensed each decade for these particular four stats.

Based on the average increase or decrease for each decade determined in the last section, an estimate is made for the values of each variable in 2030.

Then, the distribution for each variable is simulated using the 2030 estimated values using the `scipy` package. The size of each distribution is set to 250 results in the notebook. However, the user may wish to alter this value and the option is there to do so within Section 7 of the notebook (if using a dynamic version of the notebook).

A comparison is then made of each variable using the pairplot function within the `seaborn` package. 

## Credits

Historical data was gathered from the PGA Tour's website: https://www.pgatour.com/

## References

Full references for sources used are provided within the notebook.

## Contact

[Andrew Walker](mailto:G00398788@gmit.ie)




