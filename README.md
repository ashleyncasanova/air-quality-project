## **Jupyter Notebook**
___
## **Contents**

[**Notes**](#notes)

* [How to open Jupyter in a Virtual Environment](#how-to-open-jupyter-in-a-virtual-environment)

* [How to close Jupyter in a Virtual Environment](#how-to-close-jupyter-in-a-virtual-environment)

\
[**Resources**](#resources)

* [Mini Conda](#mini-conda)

* [Google Colaboratory](#google-colaboratory)

* [A gallery of interesting Jupyter Notebooks](#a-gallery-of-interesting-jupyter-notebooks)

\
[**Tools**](#tools)

* [Tools that come with Jupyter Notebook](#tools-that-come-with-jupyter-notebook)

    * [nbconvert](#nbconvert)

    * [nbformat](#nbformat)

* [Tools that do not come with Jupyter Notebook](#tools-that-do-not-come-with-jupyter-notebook)

    * [papermill](#papermill)

    * [Jupyter Notebook Extensions](#jupyter-notebook-extensions)
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

>Note: This will launch Jupyter Notebooks in a new window.

>Note: Launching Jupyter Notebooks in our home directory (~) will give us access to all of the files and directories it contains.

>Note: The ampersand (&) is not necessary, but is useful as it will run our virtual environment in the background, freeing up the terminal for other things. 
___
### [How to close Jupyter in a Virtual Environment](https://youtu.be/DKiI6NfSIe8)
Just shutting the tab does not close the notebook. It will keep running until we tell it to stop.

There are three ways we can explicitly **shut down** the notebook:
1. by going to _file_ and selecting _close and hault_
2. from the _dashboard_ by checking the box next to the notebook and clicking _shutdown_
3. from the _terminal_ by deactivating our virtual environment

 After you **save** and **shut down** your notebook, you can exit the virtual environment by closing out the terminal.  If we are still using the terminal we can just exit out of the jupiter notebooks part of it.

 Since we are running this in a background job right now, we can run the command **jobs** to show us what jobs are currently running and we can see that we have a notebook running.

 ```terminal
 jobs
 ```

 In this case we can use the command **kill** (to kill a background job or process) followed by %1. This will kill the jupiter notebook.

 ```terminal
 kill %1
 ```

 At this point you may want to re-run jobs, to check that there are no more jobs running.

 If you are not back in your home directory you can deactivate the virtual environment using **conda deactivate**.

 ```terminal
 conda deactivate
 ```

 This should return you to your home directory (~).

 >Note: If we did not use the ampersand (&), then we can use **control-c** to stop the server.
___
### **Resources**

### [Mini Conda][2]
* It is a small, bootstrap version of Anaconda that includes only conda, Python, the packages they depend on, and a small number of other useful packages, including pip, zlib and a few others.

### [Google Colaboratory][3]
* Similar to Jupyter Notebooks, except it runs in the browser.

### [A gallery of interesting Jupyter Notebooks][4]
* A curated collection of Jupyter/IPython notebooks on GitHub.

___
### **Tools**

### **Tools that come with Jupyter Notebook**

### [nbconvert][5]
* Converts notebooks to other formats.

### [nbformat][6]
* [Python API for working with notebook files][7]
    * A way to progromatically work with notebook files within python script.


### **Tools that do not come with Jupyter Notebook**

### [papermill][8]
* Lets you parameterize (pass variables into) and execute notebooks.

### [Jupyter Notebook Extensions][9]
* Any functionality you want may exist with a jupyter notebook extention.
* The documentation for all maintained extentions can be found [here](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/).
___
[1]: https://www.youtube.com/watch?v=DKiI6NfSIe8&t=175s
[3]: https://colab.research.google.com/notebooks/intro.ipynb
[2]: https://docs.conda.io/en/latest/miniconda.html
[4]: https://gist.github.com/ocoyawale/54d92fd4bf92508a2a6e482b5fa480fd
[5]: https://nbconvert.readthedocs.io/en/latest/
[6]: https://nbformat.readthedocs.io/en/latest/
[7]: https://nbformat.readthedocs.io/en/latest/api.html
[8]: https://papermill.readthedocs.io/en/latest/
[9]: https://github.com/ipython-contrib/jupyter_contrib_nbextensions