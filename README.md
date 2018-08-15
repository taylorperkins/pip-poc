# pip-poc
Small repo for a pip poc using requirements.txt file for packages

## Pre-Req
1. [pip](https://pip.pypa.io/en/stable/installing/) Must have globally installed.
2. Some sort of virtual environment tool. I have recently been using [virtualenvwrapper](http://virtualenvwrapper.readthedocs.io/en/latest/install.html) for work, but I have also had a great experience with just [virtualenv](https://virtualenv.pypa.io/en/stable/installation/). Python 3 now has `pyenv` as a builtin.
* To know you have a package installed, you can run `which <package_name>` in your terminal. For the sake of this walkthrough, I will be using virtualenv since it is so easy, and works across multiple python versions.

## Steps
1. Clone down this project! Move into the project directory after it has been cloned down.
2. Create a blank virtual environment for this project.
```bash
virtualenv --python=`which python3.6` <venv name>
```
3. "activate" your virtual environment. 
```bash
source <venv name>/bin/activate
```
* this command is slightly different on windows, the activate script lives in a different location. 
4. assert your pip library is "empty" with `pip list`
* You should still see pip, setuptools, and wheel available.
5. assert pip lives in your environment with `which pip`
6. assert python lives in your environment with `which python`
7. assert that python is the version you want (should be 3.6) with `python --version`
8. Install the packages with `pip install -r requirements.txt`
9. assert that the package updates are accurate with `pip list`
10. run `jupyter notebook --debug` in your terminal
11. Create a new file through the jupyter ui using python3
12. Import all packages in requirements.txt!!
