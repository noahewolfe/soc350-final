# Introduction

Hello! Welcome to the result of my SOC 350: Food and Society final project. Here, I have conducted a quantitative analysis centered on food access in ten North Carolina counties. In particular, I walk through an attempt to find a new metric to predict the number of low-access, low-income individuals (as defined by the USDA Food Access Research Atlas), as a vehicle for making quantitative food sociology accessible to other science, technology, engineering, and mathematics majors like myself. Although the statistical analysis itself may not have been especially insightful, and would require extra data cleaning to be rigorous, the notebooks provide an introduction to the kinds of data sociologists may think about when studying food access.

# Manifest

The inputs into, and results of, my analysis can be viewed in a browser without installing any code. There are six files or folders in this code repository;
- `analysis.ipynb`: **This is the crux of the project**, as it is the `Python` notebook that contains my statistical analysis and results! Click on it in the interface above (it should act like a link). If that doesn't work, navigate to this link: https://github.ncsu.edu/newolfe/soc350-final/blob/main/analysis.ipynb.
- `load_data.ipynb`: This notebook downloads information on stores in ten North Carolina counties from the OpenStreetMap. It is documented, but not crucial for understanding the quantitative analysis I perform in `analysis.ipynb`.
- `2019-food-access-research-atlas/`: This folder contains the 2019 USDA Food Access Research Atlas, downloaded from https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data/.
- `map.pkl`: A local copy of the data downloaded from OpenStreetMap, as it takes a little while to download the data from the OpenStreetMap!
- `README.md`: This file, describing the code repository!
- `.gitignore`: A special file that tells Github (the service hosting this code repository) to ignore extraneous temporary files that Python generates while it runs. This does not affect the quantitative analysis.


# Installation and Setup

Here, I present the steps to use this code locally, however **the `Python` notebooks are viewable in the browser without performing these steps**.

1. Download the Python interpreter; it can be downloaded from [here](https://www.python.org/downloads/). Make sure to download Python version 3.x (e.g. 3.10 is the latest).
2. After installation, open a terminal window (e.g. the Terminal app on MacOS), and run the following command:
```
pip install numpy pandas matplotlib tqdm overpy
```
This will install the third-party code libraries nessecary to make the notebook works.
3. Next, run another installation command:
```
pip install jupyter
```
This will install the `jupyter-notebook` sofware required to run the `Python` notebooks (e.g. `analysis.ipynb`) locally.
4. Finally, in the same terminal window type
```
jupyter-notebook
```
Some code will be displayed, and then it should open a browser window. In that browser window you will see a filesystem interface; navigate to the location of this repository on your computer, and open `analysis.ipynb`. From there, you can run the code in the notebook locally (see [here](https://jupyter.org/) for documentation on using notebooks with `jupyter`) and modify it as you wish. Have fun!
