### kaggle-data-analysis
### An introduction to data analysis using Python

# 1 - Setting up your environment. 
We will be using Python to process a Kaggle dataset. Before starting on the project, you will need to install a few tools:

- Anaconda
Anaconda is a distribution of packages built for data science. It comes with conda, a package and environment manager. You'll be using conda to create environments for isolating your projects that use different versions of Python and/or different packages. You'll also use it to install, uninstall, and update packages in your environments. Using Anaconda has made my life working with data much more pleasant.

Check out the following video to get started:
https://www.youtube.com/watch?v=VXukXZv7SCQ

Ensure that you install the following:
- Anaconda (as described in the video)
- Python 3
 
## 1.1 Creating your virtual environment
Run the following commands in a terminal:

    conda create -n kaggle python=3

    source activate kaggle


## 1.2 - Additional Python Libraries
It is common to store large dataset in matrices. There are a lot of libraries available that extend the basic functionality of Python. Two in particular, NumPy and Pandas allow you to easily manipulate matrix data. Matplotlib provides a suite of tools for visuallising data.

With your Kaggle environment active, run the following commands to install numpy, pandas and matplotlib in your new virtualenv set up:
    
    conda install numpy pandas matplotlib

# 2 - Jupyter Notebooks
The notebook is a web application that allows you to combine explanatory text, math equations, code, and visualizations all in one easily sharable document. Notebooks have quickly become an essential tool when working with data. You'll find them being used for data cleaning and exploration, visualization, machine learning, and big data analysis. Typically you'd be doing this work in a terminal, either the normal Python shell or with IPython. Your visualizations would be in separate windows, any documentation would be in separate documents, along with various scripts for functions and classes. However, with notebooks, all of these are in one place and easily read together.

To set up Jupyter notebook in your kaggle environment, run the following command:

    conda install jupyter notebook

# 3 - Launching the notebook server
With the kaggle environment active, enter jupyter notebook in your terminal or console. This will start the server in the directory you ran the command in. That means any notebook files will be saved in that directory. Typically you'd want to start the server in the directory where your notebooks live. However, you can navigate through your file system to where the notebooks are.

When you run the command, the server home should open in your browser. By default, the notebook server runs at http://localhost:8888. If you aren't familiar with this, localhost means your computer and 8888 is the port the server is communicating on. As long as the server is still running, you can always come back to it by going to http://localhost:8888 in your browser.

If you start another server, it'll try to use port 8888, but since it is occupied, the new server will run on port 8889. Then, you'd connect to it at http://localhost:8889. Every additional notebook server will increment the port number like this.

If you tried starting your own server, it should look something like this:

![](https://imageshack.com/a/img922/242/PVEZ5v.png)

You might see some files and folders in the list here, it depends on where you started the server from.

Over on the right, you can click on "New" to create a new notebook, text file, folder, or terminal. The list under "Notebooks" shows the kernels you have installed. Here I'm running the server in a Python 3 environment, so I have a Python 3 kernel available. You might see Python 2 here. I've also installed kernels for Scala 2.10 and 2.11 which you see in the list.

The tabs at the top show Files, Running, and Cluster. Files shows all the files and folders in the current directory. Clicking on the Running tab will list all the currently running notebooks. From there you can manage them.i

You should see the kaggle environment you created in earlier steps.

## 3.1 - Shutting down jupyter
You can shutdown individual notebooks by marking the checkbox next to the notebook on the server home and clicking "Shutdown." Make sure you've saved your work before you do this though! Any changes since the last time you saved will be lost. You'll also need to rerun the code the next time you run the notebook.

![](https://imageshack.com/a/img923/6466/SJE50n.png)

## 3.2 - Notebook interface

When you create a new notebook, you should see something like this:

![](https://imageshack.com/a/img922/5103/Lr17la.png)

Feel free to try this yourself and poke around a bit.

You’ll see a little box outlined in green. This is called a cell. Cells are where you write and run your code. You can also change it to render Markdown, a popular formatting syntax for writing web content. I'll cover Markdown in more detail later. In the toolbar, click “Code” to change it to Markdown and back. The little play button runs the cell, and the up and down arrows move cells up and down.

[![Click to view a sample execution of a cell](https://s3.amazonaws.com/content.udacity-data.com/courses/ud1111/notebook+interface.mp4)](https://s3.amazonaws.com/content.udacity-data.com/courses/ud1111/notebook+interface.mp4)

When you run a code cell, the output is displayed below the cell. The cell also gets numbered, you see In [1]: on the left. This lets you know the code was run and the order if you run multiple cells. Running the cell in Markdown mode renders the Markdown as text.

More things
At the top you see the title. Click on this to rename the notebook.

Over on the right is the kernel type (Python 3 in my case) and next to it, a little circle. When the kernel is running a cell, it'll fill in. For most operations which run quickly, it won't fill in. It's a little indicator to let you know longer running code is actually running.

Along with the save button in the toolbar, notebooks are automatically saved periodically. The most recent save is noted to the right of the title. You can save manually with the save button, or by pressing escape then s on your keyboard. The escape key changes to command mode and s is the shortcut for "save." I'll cover command mode and keyboard shortcuts later.

In the "File" menu, you can download the notebook in multiple formats. You'll often want to download it as an HTML file to share with others who aren't using Jupyter. Also, you can download the notebook as a normal Python file where all the code will run like normal. The Markdown and reST formats are great for using notebooks in blogs or documentation.

![](https://imageshack.com/a/img922/3181/PGaWf8.png)

[Here is a cheat sheet of other things you can do in a notebook session](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

# 4 -Data Analysis
Please follow some basic tutorials on NumPy, Pandas and Matplotlib - Link to be provided.

Check out this notebook which provides a guide for how to use those libraries to analyse a sample dataset: http://nbviewer.jupyter.org/github/agconti/kaggle-titanic/blob/master/Titanic.ipynb

Once you are done with that, it is your turn to choose a Kaggle dataset and perform your own analysis.
