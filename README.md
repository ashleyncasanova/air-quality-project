## **Jupyter Notebook**
___
## **Contents**

[**Notes**](#notes)

[How to open Jupyter in a Virtual Environment](#how-to-open-jupyter-in-a-virtual-environment)

\
[**Resources**](#resources)

[Mini Conda](#mini-conda)

[Google Colaboratory](#google-colaboratory)

[A gallery of interesting Jupyter Notebooks](#a-gallery-of-interesting-jupyter-notebooks)
___
### **Notes**

### [How to open Jupyter in a Virtual Environment][1]

\
Step 1: Create virtual environment (using the terminal)

```terminal
conda create -n <virtual-environment-name> <list-packages>
```
>Note: The terminal will return a package plan, listing the location of the virtual environment and any packages/associated dependencies that will be installed.

\
Step 2: Download and install ackages and dependencies

```terminal
Proceed ([y]/n)?
```
>Note: The user will be asked if they want to proceed. Review the package plan, select yes (y) and press enter.

\
Step 3: Activate virtual environment

```terminal
conda activate <virtual-environment-name>
```
>Note: The command _which python_ will show the current version of python being used.

\
Step 4: Launch jupyter notebook

```terminal
jupyter notebook &
```

>Note: The ampersand (&) is not necessary, but is useful as it will run our virtual environment in the background, freeing up the terminal for other things. 
___
### **Resources**

### [Mini Conda][2]
* It is a small, bootstrap version of Anaconda that includes only conda, Python, the packages they depend on, and a small number of other useful packages, including pip, zlib and a few others.

### [Google Colaboratory][3]
* Similar to Jupyter Notebooks, except it runs in the browser.

### [A gallery of interesting Jupyter Notebooks][4]
* A curated collection of Jupyter/IPython notebooks on GitHub

___
[1]: https://www.youtube.com/watch?v=DKiI6NfSIe8&t=175s
[3]: https://colab.research.google.com/notebooks/intro.ipynb
[2]: https://docs.conda.io/en/latest/miniconda.html
[4]: https://gist.github.com/ocoyawale/54d92fd4bf92508a2a6e482b5fa480fd