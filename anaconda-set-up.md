## How to set up your own anaconda in a scientific way?

###### python2, python3, R in conda

### Introduction

* what is anaconda?

  - According to its own website, Anaconda is the leading open data science platform powered by Python. The open source version of Anaconda is a high performance distribution of Python and R and includes over 100 of the most popular Python, R and Scala packages for data science.
  - Or you can simply regard it as a manager of the packages of your programming languages.

* why we want to use anaconda?

  - Convinient to manage packages
  - Jupyter notebook
 
* object
  - Set up anaconda for a python and r user (linux)
  - I use py2 more often so I set it my default environment

### Get started!

1. Click this [link](https://www.continuum.io/downloads) and download corresponding version of anaconda. 

2. Type the following line in the terminal and the installation will be set up automatically
        ```bash Anaconda2-4.3.1-Linux-x86_64.sh``` . 
    Do include the "bash" command even if you are not using the bash shell.

3. Add the following line to the **.bashrc** or **.zshrc**(if you are a zsh user).
        ```export PATH="/home/zijun/anaconda/bin:$PATH"```

4. Create python3 environment in your conda. 
        ```$ conda create -n py3 python=3.5 anaconda```

5. Create R environment in your conda.
        ```conda create -n r -c r r-essentials```
        
6. Install tck for R
        ```conda install -c intel tcl=8.6.4```

### Some issues you may encounter during the process
* tcl not found
> install.packages('highfrequency')  
--- Please select a CRAN mirror for use in this session ---
Error: .onLoad failed in loadNamespace() for 'tcltk', details:
call: fun(libname, pkgname)
error: Can't find a usable init.tcl in the following directories: 
/opt/anaconda1anaconda2anaconda3/lib/tcl8.5 ./lib/tcl8.5 ./lib/tcl8.5 ./library ./library ./tcl8.5.18/library ./tcl8.5.18/library

Solution: tck is a package which supports install.packages() function and it is installed in the global environment if you use ```sudo apt-get install tcl8.5-dev tk8.5-dev``` and conda has no access to it. Just do the 5th step above to solve this problem.
              or you could add following lines to the .bashrc
              ``` export TCL_LIBRARY="/home/zijun/anaconda2/lib/tcl8.5"
              export TK_LIBRARY="/home/zijun/anaconda2/lib/tk8.5" ```



