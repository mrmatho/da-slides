---
layout: cover
transition: fade
hideInToc: false
background: /img/streamlit.svg
---

# Visualisations using Streamlit, Python, Pandas and Plotly

---
layout: li
---

::li::

- To be able to interpret Streamlit, python and plotly code.
- To be able to get started with Streamlit on your own computer.

::sc::

- Install Streamlit on your own computer.
- Read and interpret the code in the example meteorites Streamlit app.
- Create your own simple Streamlit app.

---
layout: center
---

# Streamlit
<img src="/img/streamlit.svg" alt="Streamlit" style="width:400px; float:right;"/>

**Streamlit** is a Python library that allows you to create web applications for data science and machine learning projects. It is designed to be easy to use, allowing you to turn data scripts into shareable web apps quickly.

We are going to use Streamlit to allow us to add interactivity to our data visualisations. The focus of our work in not on the coding parts, but on how we put the visualisations together, and build visualisations that are meaningful.

---
layout: center
---

# Installing Streamlit

To install Streamlit, you need to have Python installed on your computer. You can check if you have Python installed by opening a terminal or command prompt and typing:

```bash
python --version
```

If you don't have Python installed, you can download it from the [official Python website](https://www.python.org/downloads/).

Once you have Python installed, you can install Streamlit using pip. Open a terminal in VS Code and type:

```bash
pip install streamlit
```

This will install Streamlit and all its dependencies.


---
layout: center
---
# Running a Streamlit App

To check that Streamlit is installed correctly, you can run a simple Streamlit app. Open a terminal in VS Code and type:

```bash
streamlit hello
```

This will open a new tab in your web browser with a simple Streamlit app that demonstrates some of the features of Streamlit.

Then you can close the tab and stop the app by pressing `Ctrl+C` in the terminal.
---
layout: center
---

# Creating a Simple Streamlit App

To create a simple Streamlit app, you need to create a Python file with the `.py` extension. Create `app.py` in your project folder.

In this file, you can write your Streamlit code. Here is a simple example:

```python

import streamlit as st

st.title("Hello, Streamlit!")
st.write("This is my first Streamlit app.")

n = st.number_input("Enter a number:", 0)
st.write(f"You entered: {n}. The square of {n} is {n**2}.")
```

To run this app, open a terminal in VS Code and type:

```bash
streamlit run app.py
```

Each time you create a streamlit app, put it in a new folder. Use `app.py` as the name of the file by convention.

---

