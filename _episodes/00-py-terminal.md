---
title: "Python Interupter in Bash"
teaching: 5
exercises: 1
questions:
- "How can I use python in the Bash Shell?"
objectives:
- "Connect the Python Lesson to the Bash Lesson"
- "Understand the limitations of running Python in Bash"
- "Justify the use of other tools for teaching and development"
keypoints:
- "There are multiple ways to interact with Python"
---
## Python can be launched from the Bash Shell
We can work in python without using a text editor or integrated development environment(ide). Instead, we can launch the Python Interputer within the Bash Shell.

Open your shell window and navigation to your data for this lesson. Enter python into the window.

~~~
$ python
~~~
{: .bash}

After enter the python command, you will enter into a python environment within the shell. Notice how your cursor changes >>>.

~~~
Python 3.5.2 |Anaconda 4.1.1 (x86_64)| (default, Jul  2 2016, 17:52:12)
[GCC 4.2.1 Compatible Apple LLVM 4.2 (clang-425.0.28)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
~~~
{: .output}

We can now start entering python. We can do simply arthimtic.

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
>>> first_name="Sarah"
>>> print(first_name)
~~~
{: .python}

~~~
Sarah
~~~
{: .output}


Working in this environment, you can use many of the same shortcuts including tab completion and the up arrow to return to previous commands.

There are several limitations to working with python in this environment. A major one is that their is no ability to save or export your work. You also cannot run multiple lines of code at once. The Python Interupter is handy for quick testing.

Writing Python in a Text Editor or Interactive Python Environment will allow to write, run, save, and re-run your python programs. Most also will provide visual clues to help you with your python syntax.

Today, we are going to be working with the juypter notebook, which is a great tool for learning. As you start to work more with python, you will find the tool that works best for you. Some popular options are Atom or Sublime Text.
