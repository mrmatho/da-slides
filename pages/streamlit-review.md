---
title: "Streamlit Review"
layout: cover
transition: fade
hideInToc: false
background: https://cover.sli.dev
---

# Streamlit Review

---
layout: center
zoom: 0.8
---

# From SAT Criterion 8 - Skills in using data visualisation software tools...

| Indicators | 1–2 (very low) | 3–4 (low) | 5–6 (medium) | 7–8 (high) | 9–10 (very high) |
|------------|----------------|-----------|--------------|------------|------------------|
| **Use of data visualisation software tools to create and present data visualisations.** | Identifies functions and formats to create infographics and/or dynamic data visualisations that incorporate: *text and images.* | Applies functions and formats to create infographics and/or dynamic data visualisations that incorporate: *text, images, symbols and charts* | Uses functions, formats and conventions to create infographics and/or dynamic data visualisations that incorporate: *a range of chart types.* | Uses functions, formats and conventions to create infographics and/or dynamic data visualisations that explain identified relationships, trends and patterns. Explains why the types of data visualisations were used | Selects and uses functions, formats and conventions to create effective infographics and/or dynamic data visualisations that clearly communicate and displays all findings to a target audience. Evaluates the use of the types of data visualisations. |

So what is important for us to be able to do in Streamlit?

<v-clicks depth="2">

- Text, images, symbols, charts
- A range of chart types
- Effective communication

</v-clicks>

---
layout: center
zoom: 1.1
---

# Text and Images

- `st.write()` for plain text
- `st.markdown()` for formatted text
- `st.image()` for images
- `st.header()`, `st.subheader()`, `st.title()` for headings

```python

import streamlit as st

st.title("Research Question")

st.subheader("Subheading")

st.markdown("This is a **paragraph** of text that *explains* the research question.")

st.image("path/to/image.png", caption="Image Caption")
```

---
layout: center
zoom: 1.1
---

# Charts

We have used plotly for our charts, but Streamlit supports many libraries if you have a particular chart or style you need.

```python
import streamlit as st
import plotly.express as px
import pandas as pd

# Load data from your spreadsheet

@st.cache_data
def load_data():
    df = pd.read_csv("path/to/data.csv")
    return df

df = load_data()

# Create a chart
fig = px.bar(df, x='Category', y='Value', title='Bar Chart Example')
st.plotly_chart(fig)
```

---
layout: center
zoom: 1.1
---

# Layout

- Columns: `st.columns()`
- Expander (for additional information you don't want cluttering up the screen): `st.expander()`

```python
import streamlit as st
# Create columns
col1, col2 = st.columns(2)

with col1:
    st.header("Column 1")
    st.write("Content for column 1")

with col2:
    st.header("Column 2")
    st.write("Content for column 2")
    with st.expander("More Information"):
        st.write("This is additional information that can be expanded.")

```

---