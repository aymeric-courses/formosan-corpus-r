---
title: "Section 1.3 Working with R Markdown files"
permalink: /docs/WorkingWithRMarkdown/
layout: single
toc: true
toc_sticky: true
sidebar:
  nav: docs
---

<p>In this section, we will focus more on one type of R scripts: R Markdown files. The reason is that we are going to use R Markdowns instead of raw R scripts from now on, so we need to know more about how R Markdown files work in addition to their potential.</p>

## 1. What are R Markdown files, and how to open one in R?

<p>R Markdown files are another type of script you can use in the Script block. They are a little bit more complex than raw R scripts because they need to be configured, but it is not complicated. In addition, the RStudio interface is very user-friendly, so there is almost no additional coding to do.<br>
But what are they good for? R Markdown files are especially interesting concerning data sharing, as in one same document (and you can choose the format of it, even PDF), you have the structure, the narration, the code and the output of it. Very trustable and very good-looking. I personally also find it useful not only for data sharing with other people, but with the future-myself who will go back to the analyses of a dataset after months of hiatus working on another project. With a raw R file, I often get lost and I might even need to rewrite it. But with an R Markdown document, I can catch up very quickly since everything is documented and ordered!</p>
<p>Now that I wish that I have convinced you on how useful R Markdown documents are, let's see how to open one. Just try to open a new script as usual, but instead of choosing "R Script", choose "R Markdown...".</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ScriptTypes.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ScriptTypes.png?raw=true"/></a>

<p>Afterwards, you will be prompted to provide some information, such as the title of the document, the name of the author(s) as well as its date. We will see in the next section how we can easily modify these pieces of information. You also have to indicate whether you want the output as an HTML, PDF or Word document... Since choosing the HTML option gives us more flexibility, let's choose this one, and you are set up!</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RMarkdown_Setup.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RMarkdown_Setup.png?raw=true"/></a>

## 2. The structure of R Markdown files

<p>Now we can turn to the structure of the R Markdown document itself. It has two main components:</p>

* The configuration lines,
* The content of the document itself.

<p>We will take the codes from <a href="https://aymeric-courses.github.io/formosan-corpus-r/docs/RStudioInterface/#32-your-first-script-some-syntax-and-vocabulary-of-r" target="_blank">Section 1.2</a> as an example to create our very first R Markdown document.</p>

### 2.2 Configuring the file: The YAML block

<p>Let's start with configuring the file: This corresponds to the first lines, or the header, of the script that you have just created. This is called the YAML part.</p>
### 2.3 Navigating the file: Titles and subtitles

### 2.4 Writing the content

#### Writing the narrative

#### Writing the code

## 3. Save, render and share

