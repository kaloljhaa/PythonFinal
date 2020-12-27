# PythonFinal
Final Python Programming Project for Object Oriented Programming 
# Summary
This code is inteded to extract data from an external source and transforms it from its raw form to manipulate numerical tables and time series and produce the first five rows of the data set. 
To accomplish this task, this code uses pandas, a data analysis and manipulation toolkit software library written for the Python programming language. It is a powerful and flexible open source data analysis that is a fundamental high-level building block for doing practical, real world data manipulation.
# Install and Run Instructions
1. Check to see if Python is downloaded by running the command:
 - python --version
 - If Python is already installed, it will generate a message with the Python version available.
2. Next, use a PIP command to install Pandas. PIP is a package management system used to install and manage software packages/libraries written in Python.
 - To install Pandas on Windows, use the command
     - pip install pandas
 - To install Pandas on Linux (OSX), open the Terminal Window (Commad+spacebar) and type the following command
     - $ python -m pip install pandas
3. Press enter and Linux will automatically download and install the packages/files required to run Pandas in Python
4. To import Pandas all you have to do is run the following code:
 - import pandas as PD
 - import NumPy as np
# Code
Open a remote file or database like a CSV or a JSONon a website through a URL or read from a SQL table/database to retrieve a dataset.
```ruby
import pandas as pd
url = "https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data"
columns = ["age", "work-class", "fnlwgt", "education", "education-num", "marital-status", "occupation", "relationship", "race", "sex", "capital-gain", "capital loss", "hours-per-week", "native-country", "income"]
data = pd.read_csv(url, names=columns, sep = ",", na_values = "?", skipinitialspace = True)
data.head()
```
This code shows the dataset for a census. By using the data.head () function of pandas, it shows the first 5 rows of the dataset. Changing this function to another function, such as data.describe or data.info will change the output of the code. For instance, data.describe will produce the numerical attributes such as age, FnlWgt, education-num, capital-gain, capital-loss, and hours-per-week. Pandas has numerous functions that will all provide a different output and a new perspective on the data.
<img width="1136" alt="Screen Shot 2020-11-22 at 7 41 59 PM" src="https://user-images.githubusercontent.com/74752610/99922038-2e979980-2cfc-11eb-972a-9caa951a7cb8.png">
# Future Proposal
A proposal I have for a future application using this code would be in regards to organizing a chart of data based on social media innovation. here are many instances where users would notice some specific random attribute of their followers and wish to find this person again. However, they don’t know who this person is or how to find them. The application would request the user’s permission to access their followers’ list and link their social media accounts to narrow down the search for this specific attribute. Since this code uses a python library that helps analyze data into different categories, this application would be able to narrow down the search for specifics. It can provide and organize so much data by just writing a couple of lines.
