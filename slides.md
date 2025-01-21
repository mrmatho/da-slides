---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Data Analytics Slides
paginate: true
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
# class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
---

# Contents

<Toc minDept=1 maxDepth=1 columns=2 />


<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
</div>

---
transition: fade-out
layout: image-right
image: https://cover.sli.dev
---

# Databases and SQL

## SQL

SQL is a standard language for storing, manipulating and retrieving data in databases.

We investigated SQL at a theoretical level during StepUp, and now we will learn how to use SQL in practice.

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/features/slide-scope-style
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

h2 {
  color: #2B90B6;
  font-weight: bold;
}

  p{
    font-size: 150%;
    line-height: 1.2em;
  }
</style>

---
layout: 
---

## GitHub CodeSpaces

We are using GitHub CodeSpaces to run our SQL exercises, using a database system called **DuckDB** in a **Jupyter notebook**. 

To access the SQL exercises, you will need to:

- Sign up for a GitHub account (if you don't have one already)
- Accept the invitation to the GitHub Classroom assignment (link is on Compass)
- Open the assignment in GitHub Classroom
- Click on the link to open the assignment in GitHub CodeSpaces
