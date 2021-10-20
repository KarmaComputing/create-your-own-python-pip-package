# How to create your own pip package example python

Being able to package your python project into a pip package is useful for distribution, and sharing with others especially if the code is generic enough to be useful in other projects).

This repo is base on the tutorial: from [packaging.python.org](https://packaging.python.org/tutorials/packaging-projects/)

This repo allows you to learn

- How do I create a python package which other people can install? (note: we skip the step of uploading/ publishing your package)
  - It's still useful to skip that step, because for local development , you can still `pip install -e <your package>`

## How to install/use

1. (Read the code) If you want to learn how to create yoru own, this might be a good example template.

2. Install this package an example: instructions are below:

- Clone this repo (e.g. /home/Documents/mypythonpackage), 
  - Then, *in a different folder* (e.g. /home/Documents/another-python-project).
- Create a python virtual env `python3 -m venv venv`
- `. venv/bin/activate`
- Now, install the python package in *ediable mode*
  e.g. `pip install -e /home/Documents/mypythonpackage`
- Now you can use your python package like any other `pip` installed package:
  - Start python interpreter, then import and use the package:
  ```
    . venv/bin/activate
    python
    from example_python_package import add_one 
    add_one(1)
  ```

Full example running:

```
(venv) $ python
Python 3.9.5 (default, Jun  4 2021, 12:28:51) 
[GCC 7.5.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> from example_python_package import add_one
>>> add_one(1)
2
>>> 

```
