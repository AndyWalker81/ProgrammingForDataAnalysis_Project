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

The R&A and USGA Distance Insights Report (2020) (https://www.usga.org/content/dam/usga/pdf/2020/distance-insights/DIPR-FINAL-2020-usga.pdf) finds that the average driving distance on the PGA Tour has shown a general increase, in particular from the early 1990s with the introduction of oversized drivers. Following this, further technological and rule innovations has led to a trend in increased distance off the tee.  

The project makes a comparison of the above four variables to:

1. Model how driving distance affects accuracy
2. Model how distance and accuracy affect the number of greens in regulation hit
3. Model how distance and accuracy affect the number of birdies scored
4. Model how the number of greens in regulation hit affects birdies

The project is described in further detail in the notebook itself.

 It is considered that it might be a useful simulation for golfers to establish if distance could be considered to be more important than accuracy, or vice versa, in the context of reaching in the green in fewer shots and scoring birdies.

## Install

Python distributions provide the language itself, along with the most commonly used packages and tools. These downloadable files require little configuration, work on almost all setups, and provide all the commonly used scientific python tools. [Anaconda](https://www.anaconda.com/download/) works on Windows, Mac, and Linux, provides over 1,500 Python/R packages, and is used by over 15 million people. Anaconda is best suited to beginning users; it provides a large collection of libraries all in one.Python comes with an inbuilt package management system, [pip](https://pip.pypa.io/en/stable). Pip can install, update, or delete any official package (https://scipy.org/install/).


## Run

[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/AndyWalker81/ProgrammingForDataAnalysis_Project/blob/main/Programming_Project.ipynb)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AndyWalker81/ProgrammingForDataAnalysis_Project/HEAD?labpath=Programming_Project.ipynb)


## Explore


## Credits


## Contact






