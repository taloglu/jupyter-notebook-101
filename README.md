# Jupyter Notebook 101

This notebook is designed for the users who has never interacted with Jupyter environment before. We will cover topics like markdowns, mix-match language usage, terminal commands as well as we will check a basic data analysis flow.

### Running the notebooks

#### With Python 2.7

    $ pip install virtualenv
    $ virtualenv venv --python=python2.7
    $ . venv/bin/activate
    $ pip install --upgrade pip
    $ pip install jupyter
    $ jupyter notebook
    

#### With Python 3.6

Download Homebrew

    $ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"    
    $ brew install python
    $ python3 -m venv venv
    $ . venv/bin/activate
    $ pip install --upgrade pip
    $ pip install jupyter
    $ jupyter notebook       

#### With Docker

To run a predefined jupyter notebook with certain packages installed choose one from:

https://github.com/jupyter/docker-stacks

As a quick start go to your local /jupyter_workbook folder and run the following command in the terminal:

    $ docker run -ti --rm -p 8888:8888 -v "$PWD":/home/jovyan/work jupyter/datascience-notebook:latest


### Turning Jupyter notebook to Slides

To generate a slide deck from the executed Jupyter notebook, the following command should be executed.

    $ jupyter nbconvert Jupyter\ Notebook\ 101.ipynb --to slides --post serve

### Jupyter Lab

    $ pip install jupyterlab