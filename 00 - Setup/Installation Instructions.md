# Python Installation Instructions

This course was written in Python 3.6.
While it may be possible to run in later versions of Python,
this is not guaranteed.
If you do not have Python installed already, we highly recommend using an Anaconda Python installation (described below).

The main Python libraries you'll use are

- numpy: library for matrix operations and general mathematical operations
- scipy: a library of modeling tools common in research and data science
- pandas: dataframes for managing complex datasets
- matplotlib: general-purpose plotting library
- seaborn: special plotting library for statistical visualization
- jupyter: "notebook" style documents for python code

### Installing Anaconda Python 3

**Anaconda Python install instructions**

Anaconda is an installation of Python that also manages multiple computing environments. You can download Anaconda from https://www.continuum.io/downloads. Select your operating system and then choose a Python version that is at least 3.6. Follow the instructions on installing for your operating system.

**Creating a ```conda``` virtual environment**

We recommend that you set up a conda virtual environment so that you are sure of your environment while working on coursework material. To do this, you'll need the environment specification file `environment.yml` from the GitHub repo.
Once you've acquired it and placed it in the appropriate folder, run the following command in the command line:
```
conda env create --file environment.yml
```

This will create a _conda_ virtual environment that has the required libraries. 
Now, whenever you want to work on NEUR299, you can run
```
source activate neur299env
```
and when you're done and want to return to your regular environment you can run
```
source deactivate
```
The virtual environment can be activated from any directory. It is simply a way to control which Python version is being used and what libraries are available.