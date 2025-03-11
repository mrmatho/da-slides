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
layout: center
---

# Streamlit App Structure

Streamlit apps are structured as a series of commands that are executed in order. Each command generates a part of the app's user interface. 

Every time user input occurs, the whole page reloads. This allows for interactivity, but it also means that you need to be careful about how you structure your app.

---
layout: center
---

# Pandas and Plotly

Our starting point for the visualisations will be to use two Python libraries: `pandas` and `plotly` . We will use Pandas to manipulate our data, and Plotly to create interactive visualisations.

Pandas is a pwoerful data manipulation library that allows you to work with data in a tabular format, meaning it is ideal for importing data from CSV or Excel files. 

Plotly is a graphing library that allows you to create interactive visualisations. It is particularly useful for creating web-based visualisations that can be embedded in Streamlit apps. Plotly allows for interactivity, such as zooming and hovering over data points to see more information as well as simple animations (but we'll hold off on them).

---
layout: center
---

# Example Streamlit App

```python

import streamlit as st
import pandas as pd
import plotly.express as px

# Set the title of the app
st.set_page_config(page_title="Meteorite Landings", layout="wide")
st.title("Meteorite Landings")

# Load the data
df = pd.read_csv("meteorites.csv")
# Remove rows with missing values
df.dropna(inplace=True)

# We could do some filtering here, but we aren't right now

# Create a scatter plot
fig = px.scatter(df, x="year", y="mass", color="fall", hover_name="name")
fig.update_layout(title="Meteorite Landings", xaxis_title="Year", yaxis_title="Mass (g)")

# Display the plot
st.plotly_chart(fig, height=800)

# Display the data
st.write("Data:")
st.dataframe(df)
```

---
