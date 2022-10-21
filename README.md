# nitin-probability-distribution
# Gaussian-and-Binomial-Distribution-Python-Package

## Summary of the Python Package
This package calculates Gaussian and Binomial Dsitribution.

## Explanation of the package
Inside the folder called `distribution_package`, you'll find another folder and a number of files. Here is a description of each
- nitin-probability-distribution, which contains the code for the distributions package including **Gaussiandistribution.py**, **Binomialdistribution.py** and **Generaldistribution.py** code.
- **setup.py** a file needed for building python packages with pip
- **__init__.py** a file needed to create a package

## Installation
- If you want to install the Python package locally to your computer, you might want to set up a virtual environment first. A virtual environment is a siloed Python installation apart from your main Python installation. 
- Type this command to create a virtual environment `python -m venv env` where env is the name you want to give to your virtual environment. You'll see a new folder appear with the Python installation named env.
- In the terminal, type `cd env` and then type `.\Scripts\activate`. You'll notice that the command line now shows (env) at the beginning of the line to indicate you are using the env virtual environment
- Now, you can type `cd ..` and then `pip install answer_python_package/.` That should install your distributions Python package.

- When adding any new functions or files to the Python Package, it doesn't know so the package needs to be upgraded. Type `pip install --upgrade nitin-probability-distribution`.

## Uploading to PyPi
- The Python package is located in the folder distribution_package
You'll need to create a setup.cfg file, README.md file, and license.txt file. You'll also need to create accounts for the pypi test repository and pypi repository. 
Don't forget to keep your passwords; you'll need to type them into the command line.

- Once you have all the files set up correctly, you can use the following commands on the command line (note that you need to make the name of the package unique, so change the name of the package from distributions to something else. That means changing the information in setup.py and the folder name

  `cd distribution_package` <br />
  `python setup.py sdist` <br />
  `pip install twine` <br />

### Commands to upload to the pypi test repository
  `twine upload --repository-url https://test.pypi.org/legacy/ dist/*` <br />
  `pip install --index-url https://test.pypi.org/simple/ nitin-probability-distribution` <br />

### Command to upload to the pypi repository
  `twine upload dist/*` <br />
  `pip install nitin-probability-distribution` <br />
  
### Implementation:
`from nitin-probability-distribution import Gaussian,Binomial` <br />
`Gaussian(10, 7)` <br />
`Binomial(0.4, 25)` <br />
