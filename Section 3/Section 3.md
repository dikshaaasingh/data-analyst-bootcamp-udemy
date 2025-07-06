## Section 3: Setting up the environment
## 10. Introduction

##  You're Expected To:
- Know what coding is
- Set up your environment independently
- Handle basic errors

---

## We'll Use: Jupyter Notebook
- Easy to use, great for data analysis
- Lets you write code + explanations in one place

---

##  What You'll Learn:
- What is programming
- How to install and use Jupyter
- How to handle errors & restart when stuck

---

##  Outcome:
By the end of this section, you'll:
- Run Python code in Jupyter
- Troubleshoot errors
- Work independently in a data analysis environment

## 11. Programming Explained in a Few Minutes

# What is Programming?

##  Objective
To understand what programming is, why it’s essential, and how it works, especially for data analysts.

---

##  Understanding the Basics

- Every day, we solve many tasks, some of which are complex enough to require **computer assistance**.
- **Computers do not understand natural languages** like English.
- They only understand **binary (0s and 1s)** — similar to a **light switch** (on/off).

---

##  What is Source Code?

- A **source code** is human-readable code written in a programming language.
- It gets **translated to machine code (binary)** by a **compiler** or **interpreter** so the computer can execute it.

###  Definition of Programming:
> *“Taking a task and writing it down in a programming language that the computer can understand and execute.”*

---

##  Programming vs Computer Science

- **Programming**: Giving instructions to a computer.
- **Computer Science**: Understanding what a computer can do in theory.
- These are different concepts; beginners often confuse them.

---

##  Choosing a Programming Language

There are over **1000 programming languages**, each with different use cases:

| Language | Ideal Use Case |
|----------|----------------|
| PHP      | Web development |
| C++      | Device and system-level programming |
| Python/R | Data science, finance, statistics |

> A good programmer **masters a few languages** rather than learning them all.

---

##  Core Skills in Programming

### 1. Problem-Solving & Abstract Thinking

- Understand the problem completely.
- Break it down into **logical, sequential steps**.
- Example:  
  - Task: Add 10 to any number input by the user.  
  - Solution: Define a function → Take input → Return input + 10.

### 2. Mechanistic Thinking

- Computers are not intuitive.  
- They **only follow exact instructions** — no assumptions, no implications.
- You must write precise, well-structured code.

---

##  Code Quality Matters

- In real-world projects, you will work with **hundreds of lines of code**.
- Code should be:
  - Clean
  - Readable
  - Meaningful (use clear variable names)
- Poor code structure → Frustrates teammates and breaks workflows.

---

##  Why Programming is Great

- It strengthens:
  - Analytical thinking
  - Logical reasoning
  - Communication of ideas to machines

> Programming is not just coding; it’s about breaking problems down and **communicating solutions to computers** effectively.

---

##  Summary

- Computers need instructions in a specific format.
- Programming is the **bridge** between human logic and machine execution.
- Good programming requires **clarity**, **structure**, and **problem-solving skills**.
Here are the **course notes** based on your transcript for the lecture about **Jupyter Notebook and Python Installation**, written in **Markdown format** for easy use in a GitHub repository:

---

###  `jupyter_and_python_setup.md`

## 12. Jupyter Introduction
#  Installing Python and Jupyter Notebook

##  Why Not Just One Python App?

- **Python is a language**, not a full application.
- To run and write Python code effectively, especially for data analysis, you need:
  - **Python (the language)**
  - **Jupyter Notebook (the interface for writing/executing code)**

---

##  What is Jupyter?

- Jupyter is a **server-client application**.
- It allows you to **write and execute code in a browser**.
- It supports **multiple languages** using kernels (Python, R, Julia, etc.).

---

##  Jupyter Architecture Overview

```plaintext
+--------------------+       +--------------------------+
|  Language Kernels  | <---> |  Jupyter Server (Backend)|
+--------------------+       +--------------------------+
        ^                               |
        |                               v
+----------------------+     +--------------------------+
|    Python Kernel     |     |   Web Browser (Client)   |
|    R Kernel          |     |   (Jupyter Interface)    |
|    Julia Kernel      |     +--------------------------+
+----------------------+
````
### Key Concepts:

* **Kernels**: Language-specific engines that execute code.
* **Clients**: Interfaces (e.g., browsers) where users write code.
* **Notebook File (.ipynb)**: Stores your code, markdown, outputs, and more.

---

##  Why Do Corporations Use Jupyter?

1. **Multi-language Support**

   * One unified interface for Python, R, Julia, PHP, etc.

2. **Rich Communication**

   * Combine code + outputs + text (markdown/figures) in one file.
   * Encourages collaboration within teams.

3. **Single File Workflow**

   * No need for separate files or tabs to execute code.
   * Outputs appear inline — easier to debug and document.

4. **File Portability**

   * .ipynb files can be shared locally or hosted on servers.
   * Great for remote teams and reproducible analysis.

---

##  Installing the Tools

We’ll use **Anaconda**, which bundles:

*  Python
*  Jupyter Notebook
*  Scientific Libraries (e.g., Pandas, NumPy, Matplotlib)

 Anaconda makes it easy to get started without manually installing packages.



## 13. Jupyter - Installing Anaconda

## 14. Jupyter - Intro to Using Jupyter

## 15. Jupyter - Working with Notebook Files


```python
x = [1,2,3,4]
x
```




    [1, 2, 3, 4]




# Jupyter Notebook Basics

##  What is a Cell?

* **Cell**: Editable field where you write code or text.
* Press `Enter` → enter **edit mode** (green border + pencil icon).
* Press `Esc` → return to **command mode** (blue left margin).

---

##  Writing and Executing Code

### Sample Code

```python
x = [1, 2, 3, 4]
x
```

### Execution Methods

* `Ctrl + Enter`: Executes the cell, stays in the same cell.
* `Shift + Enter`: Executes the cell and creates a new one below.

### Input/Output Format

* Input → `In [1]:`
* Output → `Out [1]:`

---

##  Managing Cells with Shortcuts

| Action              | Shortcut Key | Description                    |
| ------------------- | ------------ | ------------------------------ |
| Cut Cell            | `X`          | Cuts the selected cell         |
| Copy Cell           | `C`          | Copies the selected cell       |
| Paste Below         | `V`          | Pastes below the selected cell |
| Insert Above        | `A`          | Inserts a new cell above       |
| Insert Below        | `B`          | Inserts a new cell below       |
| Delete Cell         | `D` (twice)  | Deletes the selected cell      |
| Convert to Markdown | `M`          | Changes cell type to markdown  |
| Convert to Code     | `Y`          | Changes cell type to code      |

---

##  Running & Stopping Code

* You can also run a cell by clicking ▶️ (Run) in the menu.
* If a cell takes too long, click ⏹️ (Stop) to interrupt execution.
* When running: a `[*]` appears → means still processing.

---

##  Markdown Cells

* Used for documentation, comments, or instructions.
* Not executed as code.
* Useful for:

  * Explaining logic
  * Structuring notebooks
  * Adding headers and lists

### Convert to Markdown:

* Menu → Change cell type to **Markdown**
* Or shortcut: `M`

### Convert back to Code:

* Menu → Change cell type to **Code**
* Or shortcut: `Y`

---

##  Key Benefits of Jupyter

1. **Modular Execution**: Run any cell independently (no need to run all previous ones).
2. **Readable Workflow**: Use markdown to document code effectively.
3. **Efficient Iteration**: Save time by debugging or modifying just one part of code.



## 16. Jupyter - Using Shortcuts


#  Advanced Tips for Coding in Jupyter Notebooks

This lesson focuses on **shortcuts and features** that improve your efficiency while coding in **Jupyter Notebook**.

---

##  Jupyter Modes: Command vs Edit

* **Command Mode**: Allows you to manage cells (blue border).

  * Access by pressing `Esc`.
* **Edit Mode**: Allows you to edit the content of a cell (green border).

  * Access by pressing `Enter`.

>  You can identify Edit Mode by the ✏️ (pencil icon) in the top-right corner of the notebook UI.

---

##  Accessing All Shortcuts

* Press **`H`** (while in Command Mode) to open the **Keyboard Shortcuts Help window**.

  * It lists shortcuts for both Command and Edit modes.
  * To close:

    * Press `H` again
    * Or click ❌ (top-right)
    * Or click **Close** at bottom
    * Or press `Esc`

---

##  Useful Shortcuts to Remember

### 1. Toggle Output: `O`

* Hides or shows the **output** of the selected cell.
* Useful when output (e.g., tables, plots) takes up a lot of space.
* You can also double-click the gray output box to collapse it.

####  Example

```python
# Example cell
x = 3 + 5
x
```

Press `Ctrl + Enter` to execute.
Then press `O` to hide/unhide the output (`8`).

---

### 2. Toggle Line Numbers: `L`

* Adds line numbers to the code cell (great for debugging).
* Useful for long code blocks and collaboration.

#### Toggle Steps:

1. Select a code cell.
2. Press **`L`**.
3. Line numbers will appear to the left of each line of code.

---

##  Summary

| Shortcut Key | Function                 |
| ------------ | ------------------------ |
| `H`          | Open/close shortcut help |
| `O`          | Toggle cell output       |
| `L`          | Toggle line numbers      |

---

## Pro Tip

💬 You are encouraged to revisit the shortcut menu (`H`) regularly and **practice using new shortcuts** as your notebooks grow in complexity.



```python
x = 5 + 3
print (x);
```

    8
    

## 17. Jupyter - Handling Error Messages


```python
x = 7+2
```


```python
print (x)
```

    9
    


```python
print(z)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[44], line 1
    ----> 1 print(z)
    

    NameError: name 'z' is not defined



```python
prit (z)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[46], line 1
    ----> 1 prit (z)
    

    NameError: name 'prit' is not defined


## 18. Jupyter - Restarting the Kernel


```python
print(x-1)
```

    8
    


```python
print(x+1)
```

    10
    


```python
print(x)
```

    9
    
