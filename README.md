# Udacity-PythonPackage
Create and Upload a Python Package for Gaussian / Binomial Distributions
<hr/>

## How to install and get it up and running

Requirements:  Python (twine)

Video of instructions:  https://youtu.be/4uosDOKn5LI
1)  Copy all files to a directory (linux, etc.)
2)  Register and create an account on pypi.org 
3)  Go to root and type "python setup.py sdist".  This createst dist folder with tar inside.
4)  "pip install twine"
5)  "twine upload --repository-url https://test.pypi.org/legacy/ dist/*"
6)  "pip install --index-url https://test.pypi.org/simple/ thy-probability"
7)  "twine upload dist/*"
8)  From any computer:  "pip install thy-probability"
9)  From python window:  "from thy_probability import Gaussian, Binomial"


## Introduction
This python package creates the binomial and gaussian distribution class and methods.  

Note* the thy-probability name is already used on pypi.  To do this, you have to change the name of thy-probability on the install, setup.py, and directory name.
Note** The dash, '-' in the thy-probability becomes a "_" when importing with python

## Files
Generaldistribution.py - The base, abstract class
Binomialdistribution.py - Class that inherit from the base class
Gaussiandistribution.py - Class that inherit from the base class
__init__.py - Necessary for Binomial and Gaussian classes to be imported with package
