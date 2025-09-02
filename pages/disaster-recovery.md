---
title: Disaster Recovery Plans
description: Overview of disaster recovery strategies and best practices.
hideInToc: False
layout: cover
transition: fade
---

# Disaster Recovery Plans

---
layout: center
zoom: 1.1
---

# Do Now Review (5 mins)

1. List all six characteristics of data integrity.
2. Write the four laws we covered in class (not including the Notifiable Data Breaches Amendment). Identify which is federal legislation and which is state legislation.

---
layout: center
zoom: 1.3
---

# Set yourself up for success

- Today's theory is dense and important
- Take notes as we go through the slides
- As a rule of thumb: anytime you see a new heading, write it down and add at least a sentence on what is important
- Ask questions if you don't understand something
- There will be a case study at the end to help you apply what you've learned

---
layout: center
zoom: 1.3
---

# From the study design:

- features of disaster recovery plans, including:
    - evacuation
    - backing up
    - restoration
    - communication
    - testing

---
layout: two-cols-header
zoom: 1.0
---

# Why do we need each element of a disaster recovery plan?

::left::
<v-clicks depth="2">

- **Evacuation**
    - Saving lives
    - Unless you know the evacuation plan, you can't plan for what happens after
- **Backing up**
    - Backup is the centre of how we recover from a disaster
    - If you don't have a backup, you can't restore
- **Restoration**
    - Getting systems back online
    - Prioritising what gets restored first

</v-clicks>

::right::

<v-clicks depth="2">

- **Communication**
    - Unless there's a plan, communication will be chaotic
    - Who needs to be informed, and when?
    - Covers internal and external communication
- **Testing**
    - A plan is useless if it doesn't work
    - Testing identifies weaknesses in the plan
    - Testing ensures everyone knows their role
    - You want people to practice in a low-stakes environment

</v-clicks>

---
layout: center
zoom: 1.1
---

# Evacuation

- The evacuation plan is the first step in a disaster recovery plan.
- It outlines how to safely evacuate personnel from the affected area.
- It includes:
    - Evacuation routes
    - Assembly points
    - Roles and responsibilities during evacuation
    - Communication protocols during evacuation
- In an IT context, the evacuation plan may give some instructions on how to safely power down equipment to prevent data loss or damage.

---
layout: center
zoom: 1.1
---

# Backing Up

- Backing up data is a critical component of disaster recovery.
- A backup strategy should include:
    - **How often** backups are performed (e.g., daily, weekly)
    - **Where** backups are stored (e.g., offsite, cloud)
    - **Types** of backups (e.g., full, incremental, differential)
    - **Who** is responsible for managing backups (roles and responsibilities)
    - When backups are **disposed of** (e.g., after a certain period)

If a backup strategy was being written separate from a disaster recovery plan, it would also include testing and verification of backups.

---
layout: center
zoom: 1.1
---

# Restoration

- Restoration is the process of recovering data and systems after a disaster.
- The restoration plan should include:
    - **Prioritisation** of systems and data to be restored first (e.g., which systems are most time-critical)
    - **Steps** for restoring data from backups
    - **Roles and responsibilities** for those involved in the restoration process
    - **Estimated timeframes** for restoration of different systems

---
layout: center
zoom: 1.1
---

# Communication

- Communication is essential during and after a disaster.
- The communication plan should include:
    - **Who** needs to be informed (e.g., employees, customers, stakeholders)
    - **When** they need to be informed (e.g., immediately, after assessment, after restoration)
    - **How** communication will be conducted (e.g., email, phone, social media)
        - This is espcially important when regular communication channels may be down
    - **Roles and responsibilities** for those involved in communication
    - **Key messages** to be communicated

---
layout: center
zoom: 1.1
---

# Testing

- Testing the disaster recovery plan is crucial to ensure its effectiveness.
- The testing plan should include:
    - **Types** of tests to be conducted (e.g., tabletop exercises, full-scale simulations)
    - **Frequency** of testing (e.g., annually, bi-annually)
    - **Roles and responsibilities** for those involved in testing
    - **Evaluation criteria** to assess the effectiveness of the plan
    - **Steps for updating** the plan based on test results and lessons learned

- Verification of backups are ensuring that backups have run each time. They form part of the testing procedures and verification can be done manually or automatically.

---
layout: center
zoom: 1.1
---

# Updating a Disaster Recovery Plan

- A disaster recovery plan should be a *living document* that is regularly reviewed and updated.
- Updates may be needed due to:
    - Changes in technology (new systems, software updates, new or modified hardware etc.)
    - Changes in business processes
    - Lessons learned from testing or actual disasters
    - Changes in personnel or roles
    - Changes in legal or regulatory requirements
- Regular reviews (e.g., annually) should be scheduled to ensure the plan remains current and effective.

---
layout: center
zoom: 1.1
---

# The Threats that a Disaster Recovery Plan Addresses

The study design lists three types of threats to the integrity and security of data and information used by organisations:

- Accidental threats
- Deliberate threats
- Event-based threats

Which of these threats would a disaster recovery plan be most important for addressing?

---
layout: two-cols-header
zoom: 1.1
---

# Threats

::left::
- **Accidental threats**
    - Examples: Human error, system failures
    - Disaster recovery plans can help mitigate the impact of accidental threats by ensuring that data is backed up and can be restored quickly.
    - Elements of the plan such as backup, restoration, and testing are particularly relevant here. Evacuation and communication may be less relevant unless the accidental threat leads to a larger disaster.

::right::
- **Deliberate threats**
    - Examples: Cyber attacks, insider threats
    - Disaster recovery plans are *helpful* for addressing deliberate threats, especially in the context of cyber attacks that may compromise data integrity and availability.
    - All elements of the disaster recovery plan are important here, as deliberate threats *can* lead to significant disruptions that require evacuation, backup, restoration, communication, and testing. 

---
layout: center
zoom: 1.1
---

# Threats (continued)

- **Event-based threats**
    - Examples: Natural disasters (e.g., floods, fires, earthquakes), power outages, terrorism incidents, etc.
    - **Disaster recovery plans are essential** for addressing event-based threats, as these events can cause widespread damage to physical infrastructure and data.
    - All elements of the disaster recovery plan are relevant - evacuation may be necessary for safety and backup, restoration, communication, and testing are critical for recovering from the event.

---
layout: two-cols
zoom: 0.9
---

# Importance of a DR plan for Organisations

**From the study design:**

- the importance of data and information security to organisations, including:
    - safeguarding business operations
    - mitigating financial loss and reputational damage
    - compliance with legal obligations

## Safeguarding business operations

- A good disaster recovery plan gets business back on track as soon as possible

::right::

## Mitigating financial loss and reputational damage

- The time taken and quantity of data loss is likely to be the most influential factor in determining the financial and reputational impact of a disaster
- Businesses don't generally get blamed for the disaster, but responding poorly can lead to both financial and reputational damage

## Compliance with legal obligations

- Strong disaster recovery plans are a key part of compliance with each of the privacy and data protection laws we covered. Failure to have a disaster recovery plan would represent a failure to take "reasonable steps" to protect data.

---
layout: center
zoom: 0.9
---

<!-- Generated by Copilot -->

# Case Study

A medium-sized financial services business experiences a fire in its office building, causing damage to computers and loss of access to important data. 

## Questions

1. What type of threat does this represent?
2. Which element of the disaster recovery plan would come into play first (and why)?
3. Walk through how the business would use each relevant element of the disaster recovery plan to recover from the fire. *Note that some elements may be used at multiple points in the recovery process.*

---
layout: center
zoom: 0.9
---

# Summary

- A disaster recovery plan is essential for organisations to effectively respond to and recover from various types of threats, including accidental, deliberate, and event-based threats.
- The key elements of a disaster recovery plan include evacuation, backing up, restoration, communication, and testing.
- Each element plays a crucial role in ensuring the safety of personnel, the integrity and availability of data, and the continuity of business operations.
- A well-designed and regularly tested disaster recovery plan helps organisations mitigate financial loss, protect their reputation, and comply with legal obligations related to data security.
- Regular testing and updating of the disaster recovery plan is vital to ensure its effectiveness in real-world scenarios.
