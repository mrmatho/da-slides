---
layout: cover
transition: fade
hideInToc: false
title: Analysis Documentation
---

# Analysis Documentation

---
layout: li
---
::li::
- To be able to describe the key elements of analysis for a data visualisation project: 
    - functional and non-functional requirements
    - constraints 
    - scope
- To be able to identify critical and creative thinking elements in your analysis

::sc::
- I have begun to document my functional and non-functional requirements, constraints and scope for my data visualisation project
- I can describe the difference between functional and non-functional requirements, constraints and scope
- I have started to document my use of critical and creative thinking in my analysis


---
layout: center
---

# From the School Based Assessment (SBA) Guide:

<div class="note">

Criterion 2 assesses students’ skills in documenting the analysis. Students will document the data they have collected and used to inform the analysis of the research question. They also document the methods and techniques they have used to collect the data and reference how the data collected meets the characteristics of data integrity. Students then document the functional and non-functional requirements, constraints and scope of the infographics and/or dynamic data visualisations. An example of an outline for developing a research question around the requirements, constraints and scope is in the Support material.

Students will document evidence of their critical and creative thinking through critical analysis, the use of questions and follow-up questions to clarify the development of the solution requirements, constraints and scope. This is completed as part of the Analysis stage in Criterion 2. Refer to the Skills underpinning the Analysis stage in the Units 1 to 4: Problem-solving methodology specifications on page 18 of the study design.

</div>

---
layout: center
---

# Structure of your Analysis Documentation for this Criterion

- Functional Requirements
- Non-Functional Requirements
- Constraints
- Scope
- Data Collection Sources and Methods
- Evidence of Critical and Creative Thinking

These should each be sections in your analysis documentation. There is no strict limit or indication to how long each section should be, instead you should focus on using the SAT Criteria as a guide.

---
layout: fact
---

# Solution Requirements

The solution requirements of a project should clearly outline the expectations and functionalities that the project aims to achieve. This includes both functional and non-functional aspects. 

---
layout: center
---

# Functional Requirements

These describe **what** the software solution should do. 

This involves specific details such as input required, output developed and functions of the solution, including data manipulation and validation. 

In a data visualisation project, functional requirements must therefore include: 

- The data that will be used in the project
- How the data will be manipulated and validated
- The types of visualisations that will be created
- The types of interactions that will be available to the user

Some of the functional requirements come straight from the task itself and will look the same for everyone. Others will be specific to your project and research question. 

---
layout: center
---

# Non-Functional Requirements

These describe **how** the software solution should perform.

This includes aspects such as usability, reliability, performance, security and maintainability.

It is very important to think about your **audience** and the **purpose** of your project when writing these requirements. Who is likely to be interested in your research question? What do you want them to get out of your project? Your non-functional requirements should reflect that audience and purpose.

Non-functional requirements in a data visualisation project may include:

- The visualisations should be easy to understand and interpret
- Identifying the target audience for the project and ensuring that the visualisations are appropriate for that audience
- Describing how the visualisations will meet the needs of the target audience

You will most likely have fewer non-functional requirements than functional requirements.

---
layout: center
---

# Solution Constraints

Solution constraints can be described as the conditions or limitations that must be considered when designing a solution. 

These include:

- Economic (Time and Cost)
- Technical (Speed of Processing, capacity, availability of equipment, compatibility, security)
- Social (level of expertise of users)
- Legal (intellectual property, ownership of data, privacy of data)
- Usability (accessibility, usefulness, user-friendliness)

There is often some overlap between the requirements and constraints. But constraints are documenting the limitations of your project, whereas requirements are documenting what you want to achieve. 

You should ensure you document at least one constraint from each of the categories above.

---
layout: center
---

# Scope

The scope of identifies the **boundaries or parameters** of the solution.

In your scope you should describe:

- What is included in your data visualisations (an overview of your functional requirements)
- What is excluded (Anything that people could assume is included but is not):
    - Limitations of the data
    - Limitations of the visualisations
    - Areas of the topic that are not specifically covered by your research question or visualisations

---
layout: center
zoom: 1.2
---

# Data Collection Sources and Methods

- You need to document the data you have collected and how you collected it (the data collection method). This includes both primary and secondary data sources.
- Each data source needs a brief description and justification of the data's:
    - relevance to your research question
    - reliability
    - validity

---
layout: center
---

# Evidence of Critical and Creative Thinking

Students will document evidence of their critical and creative thinking through critical analysis, the use of questions and follow-up questions to clarify the development of the solution requirements, constraints and scope.

You can do this by:

- Documenting the questions you asked yourself as you developed your requirements, constraints and scope
- Identifying changes you made to your requirements after considering your first draft
- Documenting feedback you received from your teacher or others and how you used that feedback to improve your requirements, constraints and scope

---
layout: center
---

# Examples from my Analysis

*(My Research question: What effect does home ground advantage have on the outcome of an AFL match?)*

## Functional Requirements

- The data will be sourced from the Squiggle API (https://api.squiggle.com.au) and transformed into a set of CSV file.
- Data will be validated to verify accuracy of the API, through choosing a random sample of 10 games and checking the data against the AFL website.
- Additional primary data will be collected through a survey of football fans, gathering their opinions on home ground advantage.
- Data needs to include information on the home state of each team, the state of each venue, the outcome of each game, attendance, and the final score of each game.
- Data from the CSV needs to be imported into database tables with primary and foreign key relationships between tables.
- Queries linking the tables will be created to extract the data needed for the visualisations and the output of the queries will be exported to Excel spreadsheets.
- "Neutral" games will be removed from the dataset (such as most games in 2020 due to COVID-19 and games played at non-home venues).
- The data will be visualised to allow users to see the relative home ground advantage of each team, any correlations between home ground advantage and attendance, and the effect of home ground advantage on the outcome and margin of games.

---
layout: center
---

# Examples from my Analysis

*(My Research question: What effect does home ground advantage have on the outcome of an AFL match?)*

# Non-Functional Requirements

- The visualisations should be appealling to the target audience of AFL fans and be easy to understand and interpret.
- The visualisations should be interactive and allow users to filter the data by team, venue, state and year where relevant.
- Visualisations should incorporate a range of different types of graphs and charts to present the data in a variety of ways.