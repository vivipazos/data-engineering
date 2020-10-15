# Week 1 Assignment

# Part 1 - git

1. Download and install Git
    - [https://git-scm.com/](https://git-scm.com/)
2. Configure git:
    - - `git config --global user.email "you@example.com"`
    - - `git config --global user.name "Your name"`
3. Create GitHub account
    - [https://github.com/](https://github.com/)
4. Create SSH key if you need to and add it to your GitHub account
    - [Offical GitHub guide](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/connecting-to-github-with-ssh)
5. Create a new directory on your computer for your projects
6. Clone the teaching repository into your projects directory:
    - `cd <directory>`
    - `git clone <url>`

# Part 2 - Python Programming Environment

I'll recommend a combination of Anaconda, VSCode and Jupyter Notebook. If you're comfortable setting up your own Python environment without Anaconda, and/or you want to use a different editor then that is totally fine!

## Install Anaconda

Anaconda is a Python distribution and package manager. It's a good tool for quickly setting up a learning environment for Python. You can find the invidual (free) version here:

[https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)

## VSCode

This is one of the most widely used code editors nowadays and I'd recommend it if you aren't sure what to use or don't have a preference.

https://code.visualstudio.com/

## Setting up Jupyter Notebook

Jupyter Notebook is an interactive notebook interface where you can write Python code and have it run and output within the notebook. It's a great tool for experimenting and learning. It comes with its own web interface but VSCode also has native support for it and I'd recommend using that instead.

### Jupyter Notebooks in VSCode

You can follow the official guide [here](https://code.visualstudio.com/docs/python/jupyter-support). The full steps are in the guide but they should roughly be:
1. Install Anaconda
1. Install the VSCode Python extension
1. Select your Anaconda Python environment in VSCode using the command pallette - Ctrl+Shift+P -> "Python: Select Interpreter"
1. Create a blank Jupyter Notebook using the command pallette - Ctrl+Shift+P -> "Create New Blank Jupyter Notebook"

In the official guide linked above you'll find a [section](https://code.visualstudio.com/docs/python/jupyter-support#_work-with-code-cells-in-the-notebook-editor) explaining how to write and run code in the notebooks. This explains the interface and the keyboard shortcuts.

### Jupyter Notebooks web interface

Alternatively you can use Jupyter Notebooks through their web interface. You can launch it from Anaconda Navigator or by typing `jupyter notebook` on a terminal prompt. Once you're in the web interface you can navigate to your project directory and click `New > Notebook:Python` on the right hand side of the page. You can find lots of guides online explaining the interface further.

# Part 3 - CSV files with Python standard libraries

- Create a notebook in the week1 assignment directory.
- Use Python's `csv` library to read the `earthquakes.csv` file as we did in class
    - Remember you can use either the official documentation or a tutorial as a reference for how to do this
- **Challenge 1 -** Print out the times, places, and magnitude of the earthquakes that were 6 or higher magnitude
    - Remember this will require you to convert the magnitude from a string to a float
- **Challenge 2** - See if you can list only the earthquakes that happened on the date `2016-08-04`. How many of them are there?
    - **Hint**: There are two methods you can use here to filter the rows - (1) you can work with the dates as they are (as strings) or (2) you can convert them to datetime objects first.

# Part 4 - CSV files with pandas

- Create another new notebook in the week1 assignment directory
- Use the `pandas` library to read the `earthquakes.csv` file as we did in class
    - Remember you can use tutorials or the official pandas documentation as a reference
- **Challenge 1 -** Print out the 5 highest magnitude earthquakes
    - This will require sorting the dataframe by a field (`impact.magnitude`)
    - Once you have sorted it you can limit it to just the top 5 rows
- **Challenge 2** - See if you can use pandas to find the 10 most active earthquake locations (using the `location.name` field)
    - **Hint**: Close your eyes here if you don't want hints
    - **Hint1**: You can do this in 3 steps. The first is grouping by a field (pandas has a function for this)
    - **Hint2**: pandas documentation has a User Guide page on *group by aggregation* showing various aggregation functions.
    - **Hint3**: Aggregation functions will return a different data type. Use Python's `type()` function to see what that object is so you know what you are working with.
- **Challenge 3** - Use pandas to write the data from **Challenge 2** out to a csv file.
    - **Hint:** There's a simple function that does this, much like reading csv files.

# Experiment

- If you're comfortable with the content above there's another dataset in this directory (`titanic.csv`) you can experiment with. A good challenge with this dataset might be to find the survival rate of different demographics. We can look at this briefly at the start of next class to demonstrate some more features of the `pandas` library.

# Ask if you need help!

I want to set tasks that challenge you and develop your problem solving skills but I don't want you to get completely stuck or spend a long time getting frustrated or confused with something (though that actually *is* a genuine part of the coding experience). If you'd like some help or have any questions then please reach out on Slack or email and I'll be happy to give you some pointers.