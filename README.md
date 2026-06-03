# ENGR 102 Lab Topic 12 (team)
There are two deliverables for this team assignment. Please submit the files below to **Canvas**. Please include the team header information at the top of each file with the names of all contributing team members. This is a team assignment, but **everyone** must submit the files for credit. You may discuss the problems with other teams, but your submitted work must be unique. Check out the [Frequently Asked Questions](#frequently-asked-questions) below.

This week's team and individual assignments are meant to familiarize you with two of the most commonly used engineering packages in Python: `numpy` and `matplotlib`. It will also begin to give you more experience in using modules. To do this, **as a team** you will work some of the basic tutorial/intro material for each one, **and ensure that each member of the team knows how it works**.

`numpy` is a package for performing scientific computing. In particular, it offers functions and types that will allow you to create vectors and matrices, and perform linear algebra operations more easily. [The website for `numpy` is found here.](http://www.numpy.org/)

`matplotlib` is a library for creating plots, graphs, and charts. It supports a wide range of plots and graphs, and is often used for visualizing data. [The website for `matplotlib` is found here.](https://matplotlib.org/)

## Activities

0. [Check for package installation](#check-for-package-installation)
1. [numpy](#numpy)
2. [matplotlib](#matplotlib)

## Check for package installation
Both of these may already be installed on your system depending on what distribution of Python you downloaded. If you do not have `numpy` or `matplotlib`, follow the instructions below. You should first check to ensure they are installed on your system.

Create a program with two lines of code:
```python
import numpy
import matplotlib
```

and try to run this program. If the program runs without an issue (no errors), then you have both packages installed. If you get an error, then at least one is not installed. You may need to ask for help in getting this to run.

### How to install `numpy` and `matplotlib` with VS Code
<ol>
<li>Open VS Code</li>
<li>Verify you don’t have NumPy or Matplotlib installed</li>
  <ul>
  <li>Run the single line of code <code>import numpy</code> or <code>import matplotlib</code></li>
  <li>If the code runs without an error, the packages are already installed and you don’t need to do anything!</li>
  <li>You will get an error message if you don’t have them installed:</li></ul>
<li>In the terminal run the command <code>pip install numpy</code></li>
  <ul>
  <li>Wait for it to finish, it should end with <code>Successfully installed...</code></li></ul>
<li>In the terminal run the command <code>pip install matplotlib</code></li>
  <ul>
  <li>Wait for it to finish</li>
  <li>There may be a lot of output on this one, but it should end with <code>Successfully installed...</code></li></ul>
<li>Verify it worked by rerunning the code from step 2</li>
<li>Celebrate by plotting stuff!</li>
</ol>

```python
import numpy as np
import matplotlib.pyplot as plt
from random import randint
for i in range(229):
    plt.plot(randint(1,100), randint(1,100), marker=(5,1,randint(0,360)), color='w', markeredgecolor='maroon')
plt.axis('off')
plt.show()
```

## numpy
stuff

## matplotlib
stuff

## Frequently Asked Questions
1. **What's the difference between elementwise product and matrix product?** Elementwise product is the math you're used to: multiply the values in one matrix by the values in the same index location in another matrix. Matrix product (or [matrix multiplication](https://en.wikipedia.org/wiki/Matrix_multiplication)) is fancy matrix math that you will learn in a linear algebra class. You don't have to understand it right now, just know that you need to use the `@` symbol to get NumPy to do it.

2. **Activity 1 I copy/pasted the example code from NumPy's website and I get syntax errors. What gives?** Wait... you COPIED CODE? FROM THE INTERNET? Don't do that! You'll remember it better if you type it yourself! Also, the code shown on their website is written like what you would see in Jupyter notebooks or using the command line instead of a script (file). The lines that begin with `>>>` are what you execute, the lines below are the output. In your terminal, type `python` and press enter. Then try typing the lines that start with `>>>` in your console window like this:
![console window showing how to run python and portions of the numpy tutorial](lab12team_terminal.png)
Type `quit()` to return to normal.

3. **Activity 1 when I type `a.dtype.name` it outputs `int32` instead of `int64`. What's going on?** `int32` means it's an integer stored using 32 bits. `int64` uses 64 bits. You can store a much larger number with 64 bits compared to 32 bits. The output is based on the software on your machine and how much memory it's using to store the data. This stuff is beyond ENGR 102 so you don't need to understand it. Also, `itemsize` is a conversion between bits and bytes, so when you type `a.itemsize`, it's going to return whatever number you got for `dtype` divided by 8 (32 bits is 4 bytes).

4. **Matplotlib has a lot of stuff. How much do I have to memorize?** Very little! My personal philosophy is that when you eventually need to make nice plots of data, you will have access to Matplotlib's website to look up everything you need. In grad school and my previous job, I used to spend time coding up a nice plot, then save the code to reuse with future data. Code once and reuse over and over again. I expect you to be able to read code that uses the basics of Matplotlib (like the stuff in the tutorial), but nothing fancy.

5. **How do I do XXX in Matplotlib?** My advice: look at the examples on Matplotlib's website, find one that does what you want to do, click on it and look at the code. Try clicking on some of the lines of code for more information on what it does. Also check out [Matplotlib's handouts](https://matplotlib.org/cheatsheets/) and [my example video](https://tamu.video.yuja.com/V/Video?v=16309822&node=69581067&a=62181216).

Have a question you don't see here? Email your instructor!

Based upon Dr. Keyser’s Original<br/>
Revised Summer 2026 SNR
