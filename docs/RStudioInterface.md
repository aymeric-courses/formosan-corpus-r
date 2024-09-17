---
title: "Section 1.2 Introduction to the interface of RStudio and R language"
permalink: /docs/RStudioInterface/
layout: single
toc: true
toc_sticky: true
sidebar:
  nav: docs
---

Now I assume that R and RStudio are correctly installed on your computer. You can start by opening RStudio. You will see a lot of things on your screen, many blocks, many menus, and it can be quite overwhelming. No worries! This is exactly what this section is about!

<p class="notice--warning">

<strong> :book: Objectives</strong><br>In this section, you will learn more about the RStudio interface and get familiarized with it.<br> But this section is not only about presenting the interface! In addition to that, you will also get familiar with the very basics of R language.<br>

</p>

## 1. The interface of RStudio

### 1.1 General overview of the interface: Blocks, blocks, blocks and blocks

You may see the following picture on your screen after opening RStudio:

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RStudio_FirstPage.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RStudio_FirstPage.png?raw=true"/></a>

The best way to apprehend RStudio is to understand the interface as <b>blocks</b>, which are here for different purposes.

<p class="notice--danger">

:danger: When you open RStudio for the very first time, you should get something similar as in the image above, with three blocks in the same order. But it's also possible that you have something else. If that's the case, this is completely normal and this won't affect anything for the following steps!

</p>

There are four main blocks, as in the following image. I give them unofficial names so that it will be easier to refer to them. There is one block that I call the 'computer block', a second one the 'data block', a third one the 'script block', and finally the last one, the 'console block'.

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RStudio_4Blocks.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RStudio_4Blocks.png?raw=true"/></a>

You may not be able to see the 'console block' on your computer for the moment, and again, this is completely normal! Just follow the steps below.

### 1.2 The computer block

The 'computer block' is the one on the right bottom side. I call it the 'computer block' but it's actually much more than that, but let's keep it simple for the moment.<br> First, click on the Files button. You will see that there is a list of files and folders from your computer. This is actually the interface you can use to communicate and navigate directly with your computer! <br> Again, look at all the options and play with them to understand what everything's about: 1/ Click on the files. How do these open? In RStudio? Directly on your computer? 2/ Try to go to other folders on your computer using the computer block. You'll see there is no mystery, this is just like navigating on your own computer as you usually do!

### 1.3 The variable block

### 1.4 The script block

### 1.5 The console block

### Exercise: Play with your blocks!

Your four blocks are like construction toys you can play with. You can make them disappear and then reappear, you can change their size as you wish, and you can even change the background color. In other words, make RStudio your own!

This is how you can change the size of the blocks with your mouse: (GIF of changing size)

This is how you change the background color of RStudio: (GIF of changing background color)

<p class="notice--info">

<strong> Anecdote </strong> <br> I personally change the sizes of the blocks dynamically, depending on the task I'm doing. For example, if I'm writing more complex lines of codes which could be confusing, I enlarge the script block to be sure I'm not missing any parenthesis or comma. When I'm drawing plots, I make the computer block bigger to visualize more clearly what I'm doing, and it helps me to know if I want to add or change anything on the plot.<br> Everyone's experience is different, it just depends on what your preferences are. So, really, make it your own!

</p>

### Bonus: More about the script block

## 2. Libraries

### 2.1 What is the concept of the "libraries"?

### 2.2 How to install and use libraries?

## 3. Some basic elements of R language

### 3.1 First things first: The 'working directory'

### 3.2 Your first script: Some syntax and vocabulary of R

#### Basic calculations

#### Assigning variables

#### Load data from your computer to R

#### Data description and summary

#### Transforming the data: add, delete, change

#### Plotting the data

#### Save data from R to your computer

### 3.3 Common mistakes, or how to save a lot of time

<p>You will run into many error messages, these intimidating red lines in the console block telling you that something wrong happened. We can spend hours trying to figure out what to do to make the codes work. Again, no worries! This is part of the learning process, and to be honest, even experts can't avoid error messages. The most important thing is to learn from them, so that we are able to understand what the problem is, and how to solve it.</p>
<p>From my experience, there are mistakes we often make especially as first users of R. I remember that many students in the classes I attended and taught gave up on learning programming languages just because they had to spend too much time on debugging very basic mistakes, and they couldn't focus on the opportunities R can offer. Below is a non-exhaustive list of such mistakes that I may update in the future.</p>

#### I can't load the data from my computer

#### I don't have any error message, but my code won't run

#### "Variable not found", what happened?