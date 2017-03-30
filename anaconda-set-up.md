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

2. Type the following code in the terminal and the installation will be set up automatically

        ```bash Anaconda2-4.3.1-Linux-x86_64.sh``` . 

    Do include the "bash" command even if you are not using the bash shell.

3. Add ```export PATH="/home/zijun/anaconda/bin:$PATH"``` to the **.bashrc** or **.zshrc**(if you are a zsh user).

4. Now we will create python3 environment in your conda. 
    ```$ conda create -n py35 python=3.5 anaconda```
