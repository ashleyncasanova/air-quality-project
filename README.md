## **Jupyter Notebook**
___
## **Contents**

[**Notes**](#notes)

[How to open Jupyter in a Virtual Environment](how-to-open-jupyter-in-a-virtual-environment)

\
[**Resources**](#resources)


___
### **Notes**

### [How to open Jupyter in a Virtual Environment][Jupyter Notebook Tutorial]

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



___
[Jupyter Notebook Tutorial]: https://www.youtube.com/watch?v=DKiI6NfSIe8&t=175s


