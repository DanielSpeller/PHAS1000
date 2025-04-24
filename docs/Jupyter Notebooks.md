#PHAS1000 #Y1 #Programming

Jupyter notebooks allow us to mix text, code, images, tables, maths, graphs and more into a single document. This is slightly different from conventional programming where source code is stored in large text files. Jupyter notebooks are incredibly useful for doing data analysis, writing simple programs or even driving more complex programs through an interface (they are used extensively for machine learning), but you would not write a large piece of simulation software in a notebook.

## Kernel

The _kernel_ is the program which runs the code in the notebook. We will always be using the python kernel but other languages are available. The kernel runs independently of the notebook, so we can stop and restart the kernel without closing the notebook.

## Cells

Each small chunk of code or text is called a _cell_. These can be executed individually using **shift + enter** or pressing the 'play' triangle at the top of the notebook.

Cells can be executed in any order which can cause problems, for example we expect a notebook to work from top to bottom but if you execute cells out of order then the result can be different. Therefore you should always **Reset Kernel and Run All Cells** (or press the circular arrow at the top of the notebook) if you are having any problems and before you submit any work for assessment.

In the example below if we run in the wrong order then we can print `20` which is not what we might normally expect.

**Try it yourself**: There are 3 cells below.

- Execute the first cell, second cell, third cell. The print statement should print '10'.
- Now execute the second cell (`print(x)`) again. It will now print 20.

The order in which we execute the cells changes the output.

```python
x = 10
print(x)
x = 20
```

While you _can_ execute cells out of order, I strongly advise that you don't at this stage in your Python education. I want you to imagine that your Jupyter notebook is a single piece of code that runs, logically, from top to bottom. With the exception of functions (which we will cover in a few weeks), what this means is that nothing that happens further down in the script can affect anything that happened above it; there is a very clear order of progression through the code :)

### Cell Types

The main cell types are:

- Input:
    - Code
    - Markdown
- Output

Code cells are run by the kernel. This is where you will write your python.

Markdown cells are for writing text and mathematics; like a text file but a little bit more sophisticated. You will not be writing your own markdown in this module, or assessed on it, but all my instructions are written in these.

Output cells contain output from code cells.

By default jupyter will use the last statement in a cell for any output. If we want to produce more output we should explicitly print the output. In other word, the print() statement forces Jupyter to print the output to the screen.
```python
"I will NOT be printed"`
"I will be printed"
```
```python
print("I will be printed")
print("I will also be printed")
```
It is **very important** you understand that printing the last line is a **jupyter-specific behaviour**. You must not rely on this behaviour. If you need to print, always use the `print()` function. If you need to return a value from a function use `return` (this will make more sense in a few weeks time).

# Adding New Cells

You can add cells to the notebook using the '+' button at the top of the workbook. By default it will be a 'Code' cell. You can choose a different type from the dropdown menu above (along the bar with the "Play" button).

If is very useful to add code cells to test if something works the way you expect. You may want to add markdown cells to make notes to yourself during the lectures.

**Try it yourself**: Below this cell (before the heading "Undo"):

- Insert a new cell and change the type to "Markdown". Write yourself a few notes.
- Insert a new code cell below your Markdown cell and write `2+2`. Execute and check you get the correct answer.

# Undo

There are two types of undo in jupyter.

- You can undo something inside a cell (e.g. undo some typing, undo deleting text). This is in the menu 'Edit > Undo'.
- You can undo 'cell operations'. For example if you accidentally delete a cell, you can get it back using 'Edit > Undo Cell Operation'.

**Try it yourself**:

- Delete one of the new cells you added above by clicking the cell and then 'Edit > Delete Cells'.
- Get the cell back again using 'Edit > Undo Cell Operation'.

## Code comments

In computer code we can add extra information which is not _executed_ as part of the program. These are called comments. In python they start with `#` and will be highlighted in a different colour. In these notes I will use them to describe what is happening on a particular line of code to make examples clearer. It is good practice to write comments into your own code to remind yourself and describe to others what you are doing. Coding can get quite complex, and so descriptive comments are incredibly useful.

```python
# this is a comment
"this is NOT a comment"
```

## Syntax highlighting

Different parts of the code are coloured differently. This is called syntax highlighting. This does not affect the way that the code runs but is designed to make it easier to read. Imagine if you read a book and all the verbs were one colour and the nouns another colour, this is basically what is happening. It can help us to identify errors because it identifies what is being considered a variable, a number, a function and so on.

```python
def gaussian(x, amplitude=1, center=0, width=1):
    """
    returns the value of a Gaussian with given amplitude, center and width at a point x
    """
    return  amplitude * np.exp(-(x - center)**2 / (2 * width)**2)
```

## Error messages

Python (our programming language) is a very strict language. If you make a mistake in the syntax (grammar) then it will not work and an error message will be printed. It takes time and experience to understand error messages. They provide information to us to find the error but are written quite formally meaning you have to understand a lot about programming to decipher them. If you are getting unexpected errors and cannot solve them then please ask a demonstrator for help in the workshops. When asking for help you should describe what you are trying to achieve, what result you expected and what the error message is. We will spend some time in the module looking at error messages and how to understand them.

In the cell below, change the word "foo" to "bar" and see what happens when you run the cell.

In [ ]:

foo = "I exist!"
print(foo)

## Testing your anaconda install

If you have installed anaconda on your own computer you can double check all the packages we need are installed properly by executing the cell below.

- If you get a red error message then please ask for help.
- If the output prints successfully, check the numbers. Your python version should start with a 3 and your numpy version should start with a 1. If not, then please ask for help.

In [ ]:

import numpy as np
import platform

print(f"Python Version: {platform.python_version()}")
print(f"Numpy Version: {np.version.version}")

## This is all very abstract. Why are we doing programming?

It might seem a little bit strange right now, all this printing and commenting and cell usage and stuff. But run the cells below, and see why we might want to learn to program.

The bit of code below is plotting some experimental data and comparing it to a theoretical function. Don't worry if you don't understand it right now, but have a think about what each cell is doing by reading the comments, and ask questions in the workshops! I promise you, you will have learned how to do all of this over the course of the next semester...and you'll never have to plot another graph by hand again

```python

# A cell for importing libraries (you'll learn about this continuously through the module)
import numpy as np
from matplotlib import pyplot as plt



# A cell for defining a function. Maybe you recognise the second line?
# You'll learn about functions in Week 3
def y_SUVAT_Trajectory(time, y0, uy):
    y = y0 + uy*time - 0.5*9.81*time**2
    return y



# A cell for defining our data (we might have measured this from an experiment we've done, say, in labs)
# You learn about lists in Week 5, and numpy arrays in Week 9
timeData = np.array([0.0,1.0,2.0,3.0,4.0,5.0,6.0,7.0,8.0,9.0,10.0])
yData = np.array([0.56,46.46,87.05,111.98,122.94,132.07,122.31,117.33,90.61,58.26,11.63])


# A cell for defining our constants and theoretical predictions
# You'll learn about defining variables in Week 2
initialYSpeed = 50.0
initialHeight = 0.56

yTheory = y_SUVAT_Trajectory(timeData, initialHeight, initialYSpeed)



# A cell for plotting. You'll learn about this in Week 10
plt.plot(timeData, yData, "bX", label = "Experimental Data")
plt.plot(timeData, yTheory, "--g", label = "Theoretical Prediction")

# Add annotations and labels to the graph
plt.xlabel("Time (s)")
plt.ylabel("Height (m)")
plt.title("Trajectory Data")

plt.legend()

# Uncomment the line below, and your graph will be saves as an image and put in the same folder as this script
#plt.savefig("myFirstPythonGraph.png", dpi=100)

# Show the graph here in the notebook
plt.show()
```

So there we go. 18 lines of code, and we have a beautifully formatted graph. With the addition of about 10 more lines, I could plot as many graphs as I needed automatically, depending on the amount of experiments I done. But that's loops, we'll learn about that in Week 5...

---
