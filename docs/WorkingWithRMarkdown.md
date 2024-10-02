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

<p>R Markdown files are another type of script you can use in the Script block. They are a little bit more complex than raw R scripts because they need to be configured, but it is not complicated. In addition, the RStudio interface is very user-friendly, so there is almost no additional coding to do.<br> But what are they good for? R Markdown files are especially interesting concerning data sharing, as in one same document (and you can choose the format of it, even PDF), you have the structure, the narration, the code and the output of it. Very trustable and very good-looking. I personally also find it useful not only for data sharing with other people, but with the future-myself who will go back to the analyses of a dataset after months of hiatus working on another project. With a raw R file, I often get lost and I might even need to rewrite it. But with an R Markdown document, I can catch up very quickly since everything is documented and ordered!</p>

<p>Now that I wish that I have convinced you on how useful R Markdown documents are, let's see how to open one. Just try to open a new script as usual, but instead of choosing "R Script", choose "R Markdown...".</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ScriptTypes.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ScriptTypes.png?raw=true"/></a>

<p>Afterwards, you will be prompted to provide some information, such as the title of the document, the name of the author(s) as well as its date. We will see in the next section how we can easily modify these pieces of information. You also have to indicate whether you want the output as an HTML, PDF or Word document... Since choosing the HTML option gives us more flexibility, let's choose this one, and you are set up!</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RMarkdown_Setup.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RMarkdown_Setup.png?raw=true"/></a>

<p>Before getting into the file itself, some words must be said concerning the header. At one place, you can see two buttons, "Source" and "Visual". Clicj on "Visual", and you will see many options unfolding on the right.</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RMarkdown_Headers.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RMarkdown_Headers.png?raw=true"/></a>

<p>We will mainly use three options:</p>

1.  <strong>Source / Visual:</strong> You have two ways to visualize the script you will be writing. The "Source" option allows you to see and write the codes directly. The advantage is that it gives you full control on what you are doing. The drawback is that you have to know how to code everything, and the interface is not very appealing. The "Visual" option allows you to write the script as if you were in a text editor like Word. It is intuitive and you can see what is happening while you are writing. The drawback is that sometimes it is hard to navigate inside the document because the underlying codes are doing something that is not visually represented... In that case, my strategy is to switch to the "Source" mode, make the changes that I want, and then switch back to the "Visual" mode!
2.  There is an option with the word "Normal" on it. When you click on it, other options (Header 1, Header 2, etc.) will appear. These are important to define the level of navigation of your document: "Normal" is just for the text you are writing, "Header 1" for the main title, "Header 2" for the second main title, etc.
3.  Another button is called "Insert". Indeed, we have only talked so far about how to add text and titles, but you will have to insert other elements, such as R codes. Of course, you can directly write the codes as normal text, but Markdown files can do much more! Click on "Insert", and you will see what you can add. There is a suboption called "Code Chunk": This is how you can insert R codes.

<p class="notice--info">

<strong>Time for you to play around!</strong><br> There are many more options, and there is no point in describing all of them here as we will mainly use only these three ones above. However, I encourage you to try everything and see what is happening. Try to write something, change the size, change the font. Click on the buttons. There will be error messages, but that's ok. Try to understand these errors if possible. Check any changes that occurred. Again, make these Markdown files your own!<br>

</p>

## 2. The structure of R Markdown files

<p>Now we can turn to the structure of the R Markdown document itself. It has two main components:</p>

-   The configuration lines,
-   The content of the document itself.

<p>We will take the codes from <a href="https://aymeric-courses.github.io/formosan-corpus-r/docs/RStudioInterface/#32-your-first-script-some-syntax-and-vocabulary-of-r" target="_blank">Section 1.2</a> as an example to create our very first R Markdown document.</p>

### 2.1 Configuring the file: The YAML block

#### 2.1.1 Basic features of the YAML block

<p>Let's start with configuring the file: This corresponds to the first lines, or the header, of the script that you have just created. This is called the YAML part. It looks like this so far:</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/Markdown_YAML.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/Markdown_YAML.png?raw=true"/></a>

<p>
You will remark that there are pre-filled information, such as the title of the document, the name(s) of the author(s), the date and the output format. These are what we were prompted to fill when creating the document! Now you can try to change some things, for instance:</p>
1. <strong>Title:</strong> Change to "My first R Markdown script"
2. <strong>Author:</strong> Change to you name
3. <strong>Date:</strong> Change to the date you wish, or even delete this line if you do not wish to add a date

#### 2.1.2 More advanced features of the YAML block

<p>You can also add other pieces of information, for instance:</p>

1. <strong>Date:</strong>
<p>You have more options, such as defining the format of the date, and maybe more interestingly, create a variable such that you do not have to change the date anytime you are saving the document. In other words, you may want to have a line specifying something like "This document was last modified on 'Year-Month-Day'". Just write as follows:</p>
```
date: "This document was last modified on `r Sys.Date()`"
```
<p>The code `r Sys.Date()` will look at the date of the system of your computer.</p>

3. <strong>Table of contents:</strong>
<p>The addition of titles in the document is here to help when navigating it. You can also add a table of contents such that it is even easier to navigate. You can also specify how many layers you want to display in the table of contents.</p>

```
toc: true
toc-depth: 4 ## Change this value depending on how many layers you wish to display
```

4. <strong>Format:</strong>
<p>For now, the output format is "html". Just replace with other values according to the output format you want (for example: "pdf_document").</p>

<p>In the end, the YAML block should look like this:</p>
```
---
title: "My first R Markdown script"
author: "Aymeric Collart"
date: "This document was last modified on `r Sys.Date()`"
output: pdf_document
toc: yes
toc-depth: 4
---
```

### 2.2 Navigating the file: Titles and subtitles

### 2.3 Navigating the file: Titles and subtitles

### 2.4 Writing the content

#### 2.4.1 Writing the narrative

#### 2.4.2 Writing the code

## 3. Save, render and share
