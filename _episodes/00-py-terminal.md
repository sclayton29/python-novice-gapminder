---
title: "Python Interpreter in Bash"
teaching: 5
exercises: 0
questions:
- "How can I use python in the Bash Shell?"
objectives:
- "Connect the Python Lesson to the Bash Lesson"
- "Understand the limitations of running Python in Bash"
- "Justify the use of other tools for teaching and development"
keypoints:
- "There are multiple ways to interact with Python"
- "The Python Interputer within Bash is useful for testing, but has limitations"
- "You will want to work with a IDE or Text Editor to write Python"
---
## Understanding our data
Before we dive into python. Let's look at our data. First, navigate to the directory where you saved your data. The data should be in the gapminder-py folder and in the data directory. Once you are in data run a ls to see all of your files.

~~~
$ cd gapminder-py/data
$ ls
~~~
{: .bash}

You should see six csv files. Take a closer look at the gapminder_gdp_oceania.csv file by using cat.

~~~
$ cat gapminder_gdp_oceania.csv
~~~
{: .bash}

~~~
country,gdpPercap_1952,gdpPercap_1957,gdpPercap_1962,gdpPercap_1967,gdpPercap_1972,gdpPercap_1977,gdpPercap_1982,gdpPercap_1987,gdpPercap_1992,gdpPercap_1997,gdpPercap_2002,gdpPercap_2007
Australia,10039.59564,10949.64959,12217.22686,14526.12465,16788.62948,18334.19751,19477.00928,21888.88903,23424.76683,26997.93657,30687.75473,34435.36744
New Zealand,10556.57566,12247.39532,13175.678,14463.91893,16046.03728,16233.7177,17632.4104,19007.19129,18363.32494,21050.41377,23189.80135,25185.00911
~~~
{: .output}

As we can see our data is a spreadsheet with historical GDP for individual countries. Now that we understand our data a bit better, let's move onto python.

## Python can be launched from the Bash Shell
We can work in python without using a text editor or integrated development environment(ide). Instead, we can launch the Python Interpreter within the Bash Shell.

Open your shell window and navigation to your data for this lesson. Enter python into the window.

~~~
$ python
~~~
{: .bash}

After enter the python command, you will enter into a python environment within the shell. Notice how your cursor changes.

~~~
Python 3.5.2 |Anaconda 4.1.1 (x86_64)| (default, Jul  2 2016, 17:52:12)
[GCC 4.2.1 Compatible Apple LLVM 4.2 (clang-425.0.28)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
~~~
{: .output}

We can now start entering python. We can do simple arthimtic.

~~~
>>> 3+5
~~~
{: .python}

~~~
8
~~~
{: .output}

Or assign and call variables

~~~
>>> first_name="Jane"
>>> last_name ="Smith"
>>> print(first_name)
~~~
{: .python}

~~~
Jane
~~~
{: .output}


Working in this environment, you can use many of the same shortcuts including tab completion and the up arrow to return to previous commands. Print the first_name and last_name using tab completion. You need to separate the variables with a comma.

~~~
print (first_name, last_name)
~~~

## Limitations of the Python Interpreter

There are several limitations to working with python in this environment. A major one is that their is no ability to save or export your work. You also cannot run multiple lines of code at once. The Python Interpreter is handy for quick testing.

Quit the Python Interpreter using Ctrl-D. Now, re-open the interpreter and try to call the last_name variable you created in your last session.

~~~
>>> python
>>> print (last_name)
~~~
{: .python}

~~~
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'last_name' is not defined
~~~
{: .output}

You recieve a traceback error because your work is not saved between sessions.

Writing Python in a Text Editor or Interactive Python Environment will allow to write, run, save, and re-run your python programs. Most also will provide visual clues to help you with your python syntax.

Today, we are going to be working with the juypter notebook, which is a great tool for learning. As you start to work more with python, you will find the tool that works best for you. Some popular options are Atom or Sublime Text.

To exit the Interpreter, you need to press Ctrl-D or enter quit().
