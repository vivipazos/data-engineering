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

# Part 2 - Anaconda & Jupyter Notebook

1. Install Anaconda Individual Edition - [https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)
    - Anaconda is a Python distribution and package manager. It's a good tool for quickly setting up a learning environment for Python.
2. Create a new Jupyter Notebook and get comfortable with the format and interface. You can either use VSCode or you can use the Jupyter Notebook web interface. I like VSCode personally but it's up to you.
    - To use VSCode follow the official guide here:
        - [https://code.visualstudio.com/docs/python/jupyter-support](https://code.visualstudio.com/docs/python/jupyter-support)
    - Alternatively you can launch the Jupyter Notebook web interface through Anaconda Navigator or by typing `jupyter notebook` on a terminal prompt (this should work on both OSX and Windows). Once you're in the web interface you can navigate to your project directory and click `New > Notebook:Python` on the right hand side of the page.

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

# Ask if you need help!

I want to set tasks that challenge you and develop your problem solving skills but I don't want you to get completely stuck or spend a long time getting frustrated or confused with something (though that actually *is* a genuine part of the coding experience). If you'd like some help or have any questions then please reach out on Slack or email and I'll be happy to give you some pointers.