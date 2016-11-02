---
title: "Using Python in Bash"
teaching: 10
exercises: 0
questions:
- "How can I use python in the Bash Shell?"
objectives:
- "Connect the Python Lesson to the Bash Lesson"
- "Understand the limitations of running Python in Bash"
- "Justify the use of other tools for teaching and development"
keypoints:
-"There are multiple ways to interact with Python"
---
## Python can be launched from the Bash Shell
We can work in python without using a text editor or integrated development environment(ide). Instead we can launch python from our Bash Shell.

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

There are several limitations to working with python in this environment. To demonstration, let's write a loop. We will cover python loops in more detail later in this lesson. 
