## Data Analytics and Visualization - Tech Interview Questions

### Analytics Experience 

1. Talk to me about a project you've completed involving data analytics or visualization that you are most proud of.

2. Talk to me about a project you've completed involving data cleanup. What did the data look like coming in. What steps did you need to take to clean the data?

3. Which of the following languages would you consider yourself stronger in: Python or JavaScript?

### Python 

3. (Basic) What does it mean for an object to be "iterable" in Python? What are two examples of iterable objects in Python?

    - Iterables are objects that can be iterated over -- as in a for loop. This means that we can run code repeatedly as we step through it's elements.

    - Examples of iterable objects include: Lists, Tuples, Set, Frozenset

4. (Basic) What is the difference between a "list" and a "dictionary" in Python? When might you use one vs. the other?

    - A list is a data structure that stores elements in defined order. (i.e. We add elements to a list in a specified order. Index 0 stores a particular value. Index 5 stores a particular value. Note: Lists are called "arrays" in JavaScript).

    - A dictionary is a data structure that stores elements in key-value pairs. (i.e. The key "name" may relate to the value of "Joan of Arc", the key "age" may relate to the number 15. Note: Dictionaries are similar to "objects" in JavaScript).

5. (Basic) What method would you use to add elements to a "list" in python?
    
    `.append` as in:
    
    ```python
    a = [5, 4, 3, 2] 
    a.append(6)
    ```

6. (Medium) How would you describe what a module is to a novice developer? How would you describe what a package is? How would you include a Python module in an application? How would you include a Python package in an application?

    - A module is simply a Python source file that exposes classes, functions, and global variables. 

    - A package is a directory filled with Python modules.

    - We include Python modules in an application using the `import` command at the start of our code.

    - We include Python packages in an application, by first adding a file named `__init__.py` into a folder directory. This tells Python that the folder is to be treated as a Python package. We then import the directory using the `import` command at the start of our code. 

7. (Medium) How might you write Python code for interacting with a RESTful API? Specifically what Python library might you use to execute HTTP messages?

    - The Python `requests` library allows us to create HTTP requests. 

    - To use the `requests` library we simply import the module into our application. We then specify the query url, HTTP method (GET, POST, etc.), and any authentication necessary. Example:

    ```python
    import requests
    r = requests.get('https://api.github.com/user', auth=('user', 'pass'))
    r.json()
    ```

8. (Hard) What are the essential data structures in Python Pandas? What advantages do they afford for data analysts?

    - Python Pandas introduces the Series, DataFrame, and GroupBy Objects. (They key data structure is the DataFrame).

    - DataFrames are a programmatic version of spreadsheets. They provide a host of functions for interacting with spreadsheets based on index, column, conditionals, and more. They allow a data analyst to quickly manipulate and explore large datasets. 

8. (Hard) What exactly is a Jupyter notebook? Why is it useful for data analysts?

    - Jupyter Notebooks are an alternative method for writing Python applications that involve data manipulation and exploration. Unlike the traditional IDE, Jupyter Notebook allows a developer to execute short lines of Python code and immediately see the output in real time. (No need for debugging, the output displays the moment you execute a statement block-by-block). 

    - Jupyter is particularly helpful for data analysts as it allows them to execute short blocks of code whereby they manipulate datasets and immediately see a visual representation of the tables produced. It is further useful in that Jupyter notebooks can be shared across analysts, allowing others to review the code, output, and commentary. 

    - An example Jupyter notebook can be found [here](http://nbviewer.jupyter.org/github/Jay-Oh-eN/happy-healthy-hungry/blob/master/h3.ipynb).

10. (Hard) What Python library might one use to build a plot (pie chart, scatter plot, or otherwise)?

    - The most common plotting libraries in Python include: Matplotlib, Seaborn, ggplot, Bokeh, and Plotly

11. (Hard) What exactly do the Python libraries Beautiful Soup and Scrapy do? How do they work at a high-level?

    - Beautiful Soup and Scrapy are "web scraping" libraries.

    - Both libraries work by providing developers with a means of selecting DOM elements based on HTML tags. Once selected these text elements can be stored in variables and utilized in Python applications.

### JavaScript

### HTML / CSS

### Databases

### VBA

### Advanced Topics

### Basic Statistics

### Critical Thinking Ability

1. 


