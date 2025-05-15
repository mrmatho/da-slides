---
layout: cover
transition: fade
hideInToc: false
title: Data Management Planning 
background: https://cover.sli.dev
---

# Data Management Planning

---
layout: li
---

::li::

- To be able to identify the purpose of backup, archiving and data disposal as part of a data management plan
- To be able to apply backup, archiving and data disposal to your own data analysis project

::sc::

- Write a data management plan for your SAT project

---
layout: center
zoom: 1.4
---

# Data Management

- Data management is part of maintaining the integrity of data and ensuring it is being used ethically and appropriately.
- Data management incorporates collection of data, as well as:
    - Backup
    - Archival
    - Disposal

---
layout: center
---

# Backup

Backup is the process of creating copies of data to protect it from loss or corruption.

<div class="note">

## From the study design:

The process of making a copy of data and storing the copy separately to the original data in case it is needed due to data loss. Backed up data can be full (entire copy of data), differential (changes since last full backup), incremental (changes since last backup) or a combination of these. Backups can either run manually or be scheduled to run automatically, and can be stored on a local hard drive (distinct from the original source), on external storage devices or by using cloud computing. Backups are restored when data loss occurs.

</div>

---
layout: center
---

# Backup Types

|Full|Incremental|Differential|
|---|---|---|
| A complete copy of all data|Only the data that has changed since the last backup|Only the data that has changed since the last full backup|
| More storage space required|Least storage space required|Less storage space required|
| Longer to backup|Shortest to backup|Shorter to backup|
| Restoring only needs the last backup|Restoring needs the last backup and all incremental backups|Restoring needs the last full backup and the last differential backup|

---
layout: center
---

# Backup Strategy

A backup strategy needs:
- **Frequency**: How often will backups be made? Daily, weekly, monthly?
- **Location**: Where will backups be stored? On-site, off-site, cloud?
- **Type**: What combination of backup types will be used? Full, incremental, differential?
- **Retention**: How long will backups be kept? Days, weeks, months?

<div class="note">

For our SAT project, the data is unlikely to need to change regularly or be particularly large, so a full backup stored after each lesson during data manipulation would be sufficient. This could be stored on a USB drive or in the cloud. Your backups could also act as evidence of your data manipulation process, so it is a good idea to keep them for the duration of your project.

</div>

---
layout: center
---

# Archiving

Archiving is the process of moving data that is no longer actively used to a separate storage location for long-term retention.

<div class="note">

## From the study design:

The process of moving data from a system that no longer needs to be accessed regularly to a less frequently accessed storage area for future use or to meet compliance requirements. This ensures that data can be stored separately to systems for long periods of time without impacting on current performance or storage requirements.

</div>

---
layout: center
---

# Purpose of Archiving

Regularly archiving data can help to:
- Free up space on primary storage systems
- Improve system performance
- Ensure compliance with data retention policies
- Preserve data for future reference or analysis

<div class="note">

Your data management plan should include a plan for archiving your data. This should be relatively simple for your SAT project: keeping original copies of data in a separate location to the working copy of the data. Once you have moved from working in the database to working in the spreadsheet, keeping a copy of the database could be considered archiving.

</div>
---
layout: center
---

# Disposal

<span class="note"> The study design doesn't give us a definition for disposal, so you're stuck with mine. </span>

Disposal is the process of securely deleting or destroying data that is no longer needed. Disposal is important for protecting sensitive information and ensuring compliance with data protection regulations. Any personal data that is collected **must be disposed of securely** when it is no longer needed. This includes deleting data from all storage locations, including backups and archives. 

---
layout: center
zoom: 1.2
---

# Secure Disposal of Data

Secure disposal of data can include:
- Deleting files and folders from all storage locations
- Overwriting data with random characters or patterns
- Physically destroying storage devices


<div class="note">

These methods are important because simply deleting files does not remove the data from the storage device. Data can often be recovered using data recovery software, so when data is especially sensitive or personal, it is important that it is disposed of in a way that makes it unrecoverable.

</div>
---
layout: center
---

# What do I need to submit?

As part of your SAT project, you need to submit a data management plan. This should include:

- What data you will be storing
- How you will back up your data (frequency, location, type, retention)
- How you will archive your data
- How you will dispose of your data (and when)
- How you will ensure that your data is secure

<div class="note">

Your data management plan should be succinct and clear. It also should be specific to your project - including your disposal plan. If none of the data you are collecting is personal or sensitive, it is fine to have a less secure disposal plan. Make sure you include a justification for any decisions made in your data management plan.

</div>

---
layout: center
hideInToc: false
---

# Coding Qualitative Data

Qualitative data is information that describes qualities or characteristics, rather than numerical values. It is often collected through interviews, observations, or open-ended survey questions, and can include things like opinions, experiences, or descriptions.

Coding qualitative data is the process of organizing and categorizing this information to identify patterns, themes, or trends. This can involve assigning labels or codes to specific pieces of data, and then grouping similar codes together to create broader categories. Coding can help researchers make sense of large amounts of qualitative data and draw meaningful conclusions from it.

<div class="note">

Not all of you will need to code qualitative data for your SAT project, but failing to code data that can/should be coded will cost you marks. If you believe you do not need to code qualitative data, you should review whether you are collecting enough data in the first place (you might be, but you should check).

</div>

---
layout: center
---

# Coding Qualitative Data

Examples of coding qualitative data approaches include:
- **Sentiment analysis**: Labeling comments as positive, negative, or neutral based on their emotion or tone
- **Thematic analysis**: Grouping data by common topics or themes
- **Content analysis**: Counting words or phrases and sorting them by meaning
- **Open coding**: Assigning labels to data without pre-defined categories, allowing for more flexibility in analysis
- **Axial coding**: Organizing codes into categories and subcategories to identify relationships between them
- **Selective coding**: Identifying core categories and integrating them into a cohesive narrative or theory

---
layout: center
---

# Coding Qualitative Data

Example of coding qualitative data:


| Comments | Code |
|---|---|
| After using it for a week, my mornings are a bit brighter. | Positive |
| I expected more, but it didn’t quite meet my needs. | Negative |
| It works as described, nothing more, nothing less. | Neutral |
| My friend keeps borrowing it, so it must be good! | Positive |
| I found myself looking for alternatives soon after purchase. | Negative |
| The price made me hesitate, but the quality is decent. | Neutral |
| It solved a problem I didn’t know I had. | Positive |
| I wish it had lasted longer before showing issues. | Negative |
| It’s not perfect, but it fits into my routine just fine. | Neutral |

---

# Coding Quantitative Data

It is less common that you might need to code quantitative data, but it is possible that it may assist in the readability of your data and data visualisations. Coding quantitative data is usually about categorising the numerical data into groups or ranges. This can help to identify trends or patterns in the data, and make it easier to analyse and interpret.

Example of coding quantitative data:
| Temperature (°C) | Category | Code |
|---|---|---|
| < 0 | Freezing | 1 |
| 0-10 | Cold | 2 |
| 11-20 | Cool | 3 |
| 21-30 | Warm | 4 |
| 31-40 | Hot | 5 |o
| > 40 | Extreme Heat | 6 |
