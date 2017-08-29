## Data Analytics and Visualization - Tech Interview Questions

### Analytics Experience 

1. Talk to me about a project you've completed involving data analytics or visualization that you are most proud of.

2. Talk to me about a project you've completed involving data cleanup. What did the data look like coming in. What steps did you need to take to clean the data?

3. Which of the following languages would you consider yourself stronger in: Python or JavaScript?

### Python 

4. (Basic) What does it mean for an object to be "iterable" in Python? What are two examples of iterable objects in Python?

    - Iterables are objects that can be iterated over -- as in a for loop. This means that we can run code repeatedly as we step through it's elements.

    - Examples of iterable objects include: Lists, Tuples, Set, Frozenset

5. (Basic) What is the difference between a "list" and a "dictionary" in Python? When might you use one vs. the other?

    - A list is a data structure that stores elements in defined order. (i.e. We add elements to a list in a specified order. Index 0 stores a particular value. Index 5 stores a particular value. Note: Lists are called "arrays" in JavaScript).

    - A dictionary is a data structure that stores elements in key-value pairs. (i.e. The key "name" may relate to the value of "Joan of Arc", the key "age" may relate to the number 15. Note: Dictionaries are similar to "objects" in JavaScript).

6. (Basic) What method would you use to add elements to a "list" in python?
    
    `.append` as in:
    
    ```python
    a = [5, 4, 3, 2] 
    a.append(6)
    ```

7. (Medium) How would you describe what a module is to a novice developer? How would you describe what a package is? How would you include a Python module in an application? How would you include a Python package in an application?

    - A module is simply a Python source file that exposes classes, functions, and global variables. 

    - A package is a directory filled with Python modules.

    - We include Python modules in an application using the `import` command at the start of our code.

    - We include Python packages in an application, by first adding a file named `__init__.py` into a folder directory. This tells Python that the folder is to be treated as a Python package. We then import the directory using the `import` command at the start of our code. 

8. (Medium) How might you write Python code for interacting with a RESTful API? Specifically what Python library might you use to execute HTTP messages?

    - The Python `requests` library allows us to create HTTP requests. 

    - To use the `requests` library we simply import the module into our application. We then specify the query url, HTTP method (GET, POST, etc.), and any authentication necessary. Example:

    ```python
    import requests
    r = requests.get('https://api.github.com/user', auth=('user', 'pass'))
    r.json()
    ```

9. (Hard) What are the essential data structures in Python Pandas? What advantages do they afford for data analysts?

    - Python Pandas introduces the Series, DataFrame, and GroupBy Objects. (They key data structure is the DataFrame).

    - DataFrames are a programmatic version of spreadsheets. They provide a host of functions for interacting with spreadsheets based on index, column, conditionals, and more. They allow a data analyst to quickly manipulate and explore large datasets. 

10. (Hard) What exactly is a Jupyter notebook? Why is it useful for data analysts?

    - Jupyter Notebooks are an alternative method for writing Python applications that involve data manipulation and exploration. Unlike the traditional IDE, Jupyter Notebook allows a developer to execute short lines of Python code and immediately see the output in real time. (No need for debugging, the output displays the moment you execute a statement block-by-block). 

    - Jupyter is particularly helpful for data analysts as it allows them to execute short blocks of code whereby they manipulate datasets and immediately see a visual representation of the tables produced. It is further useful in that Jupyter notebooks can be shared across analysts, allowing others to review the code, output, and commentary. 

    - An example Jupyter notebook can be found [here](http://nbviewer.jupyter.org/github/Jay-Oh-eN/happy-healthy-hungry/blob/master/h3.ipynb).

11. (Hard) What Python library might one use to build a plot (pie chart, scatter plot, or otherwise)?

    - The most common plotting libraries in Python include: Matplotlib, Seaborn, ggplot, Bokeh, and Plotly

12. (Hard) What exactly do the Python libraries Beautiful Soup and Scrapy do? How do they work at a high-level?

    - Beautiful Soup and Scrapy are "web scraping" libraries.

    - Both libraries work by providing developers with a means of selecting DOM elements based on HTML tags. Once selected these text elements can be stored in variables and utilized in Python applications.

### JavaScript

13. (Basic) In JavaScript, what are the major differences between `==` and `===`?

    - The `===` is a conditional check for type and value.

    - The `==` is a conditional check for just value (i.e. Ignores type).

    - `3 === 3 but 3 !== "3"`

14. (Medium) Given an array that is three elements long, how would you remove the second element without modifying the other two elements?

    - `array.splice(1)`

15. (Medium) What does NaN stand for in JavaScript and how can you test whether a value is equal to NaN?

    - `isNan(value)`

16. (Medium) What JavaScript method or library might you use to perform a GET request to a public RESTful API?

    - There are a number of options here, including: jQuery AJAX, JavaScript Fetch, D3 Request, Angular $http, etc. 

17. (Medium) If you were building a map filled with markers to indicate key locations in the dessert, how might you store the locations in a JSON object?
    
    - `{name: "Marker 1", lat: 34.00, lng: 32.00}`

18. (Medium) What is data binding and why is it important in data visualization?

    - Data binding is the concept by which data in an application is directly tied to the user interface in some way. As the underlying data in the application changes, so too will the visual representation in the UI.

    - In the case of data visualization, live feeds of data should trigger live changes in the UI. Frameworks like D3 and Angular include sophisticated handling for data binding.

19. (Medium) What is callback hell?

    - Callback hell occurs when a JavaScript function involves multiple layers of callbacks nested within one another. 

20. (Hard) Define "Constructor" in JavasScript. How would you describe an example use case of a constructor?

    - Constructors are special methods for creating and initializing objects created within a class. 

    - An example use case of a constructor would be if we needed to create multiple "car" objects. Each car object was given a set of pre-defined shared methods like drive or honk, but with user customizable colors and models. A constructor could thus be used to create the template by which all future car objects were created. 

21. (Hard) Using D3, how might you select all paragraph elements and apply a background color of alice-blue?  

    - `d3.selectAll("p").style("background-color", "alice-blue")` 

### HTML / CSS

22. (Basic) What is the CSS Box Model and what are its components?

    - The CSS Box Model is a way of representing all HTML elements in the form of boxes in the DOM.

    - The CSS Box Model is composed of an element, it's padding, border, and margin.

23. (Basic) Explain the concept of "flow" in HTML/CSS. What happens when a block element is floated to the left? What happens when no float is applied?

    - Flow is the concept of how HTML / CSS positions elements on the screen. When a block element is floated to the left it will appear on the far left of the containing element. It also means that the next element in the DOM will appear adjacent to it on the right. 

    - When no float is applied, block level elements take up the entire row. The next element, thus appears on the next line. 

### Databases (SQL and Mongo)

24. (Basic) Let's say you have a table called: "School-Records" stored in a MySQL database. How might you run a query to retrieve all data from from the "School-Records" table? How might you receive only the records for which the data in the "Grade" column was below a 70?

    - `SELECT * FROM School-Records`

    - `SELECT * FROM School-Records WHERE Grade < 70`

25. (Medium) What is the key difference between a SQL and NoSQL Database?

    - SQL Databases involve storing data in tables filled with rows and columns. Data can be retrieved by joining tables together prior to running queries.

    - NoSQL Databases involve storing data in a roughly JSON format. Data is stored in collections composed of documents. Data can involve deeply nested properties within a single document.  

26. (Medium) Explain the concept of joins in MySQL. What are the differences between an inner and outer join?

    - A join is effectively a combination of tables based on a shared values in a common set of columns.

    - An inner join involves combining the tables only where there is an exact column match. Any rows that do exist in one table but not the other will be excluded from the join. In essence this is an "intersection".

    - An outer join involves combining the data where there is an exact column match, but also including those rows without a column match. In essence, rows without a column match, will be included but filled with empty values where no associated values could be found. In essence, this is a "union".

27. (Medium) What is a SQL Injection Attack and how could we prevent it?

    - A SQL Injection attack is when a hacker gains inserts SQL commands into an unintended database access point. A classic example of this is when a hacker inserts SQL commands into a text-box in a user-interface; thus allowing them to manipulate the core database.

    - To prevent a SQL Injection attack involves using prepared statements or interface logic to thwart SQL statements from being executed.

28. (Hard) What is sharding? Why might we want to use it?

    - Sharding is a database partitioning strategy in which a database is broken into separate server instance to spread the load. 

    - Sharding is important when our dataset becomes extremely large. In these cases, storing data in a single server (no matter how powerful) will actually **decrease** performance. This is largely because read-write operations for data stored in memory are an intrinsically rate-limiting operation. By splitting datasets across multiple servers, you can take advantage of each server to perform large quantities of these read-write operations at the same time.

### Other Topics (Excel, Statistics, Hadoop, and Machine Learning)

29. (Medium) What function do VLookups and HLookups perform in Microsoft Excel? 
    
    - VLookups and HLookups are used to "look-up" values associated with one record according to another. As an example, let's say we had two tables: one filled with items and quantities and the second with items and prices. We could use a VLookup to retrieve the price associated with each item to calculate the total for each order.

    - The difference between a VLookup and an HLookup has to do with the orientation of the table we are retrieving data from. If the source data is in a horizontal table, we use an HLookup. If the source data is in a vertical table, we use a VLookup.   

30. (Medium) Define Regression

    - Regression is a modeling technique in which a relationship is established between two variables -- one being a dependent variable and the other being an independent variable. The assumption in regression is that the occurrence of one set of variables correlates with a predictable occurrence of the second set of variables.  

31. (Hard) Explain the concept of a Map Reduce. What does it have to do with Hadoop?

    - Map Reduce is a programming model for processing large data sets. The Map() procedure is for filtering and sorting. The Reduce() procedure is for summarizing the resulting sorted data into categories or counts.

    - Hadoop originally began as an open-source implementation of Google's MapReduce technology.  

32. (Hard) In traditional machine learning, what is the difference between "Supervised" and "Unsupervised" learning?

    - Supervised learning is where a "training" dataset marked by "correct answers" is provided to to establish an algorithm. The resulting algorithm is then used to predict correct answers for a non-training set. An example of this would be in a spam classifier where large examples of spam are provided to "train" an algorithm.

    - Unsupervised learning is where no "training" dataset is provided. In essence, the algorithm is provided a large dataset and tasked with identifying trends. An example of this would be an anomaly detector where a large dataset is provided and pointed differences are "caught" by the algorithm. 

### Critical Thinking Ability

33. (Hard) Let's say you are given the task of answering the question: "Which do Americans prefer more Italian food or Mexican food?" How might you most definitively answer the question if you cannot conduct live surveys and are only given 5 hours of time.

     - There can be many answers to this one, but one possible solution is to use the Yelp API to scrape the review counts and ratings of the top 20 Italian and Mexican restaurants in thousands of zip codes in the US. Once all the data is compiled, you can compare the counts and reviews for the aggregated data.

     - The key is that the interviewee engages the question and shows a creative ability to use technology to solve the problem with true rigor.  

34. (Hard) Let's say you are tasked with identifying which neighborhoods are most rapidly gentrifying (converting from traditionally poor to more affluent neighborhoods). How might you determine where this is taking place and report on your findings? 

    - There can be many answers to this one, but one possible solution is to use the Google Radar API in conjunction with the Zillow API and US Census to identify the number of coffee shops and/or upscale restaurants appearing in neighborhoods with traditionally lower-income populations.  

    - These findings could then be provided in the form of a Google Map with overlaid markers on color-coded zipcodes to indicate relative income level.

### General Comments

35. Communication

36. Passion

37. Personality

38. Quality / Amount of Questions Asked

39. Impressiveness

40. Well-Roundedness (Did they seem competent across all categories?)
