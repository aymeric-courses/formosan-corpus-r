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

:warning: When you open RStudio for the very first time, you should get something similar as in the image above, with three blocks in the same order. But it's also possible that you have something else. If that's the case, this is completely normal and this won't affect anything for the following steps!

</p>

There are four main blocks, as in the following image. I give them unofficial names so that it will be easier to refer to them. There is one block that I call the 'computer block', a second one the 'data block', a third one the 'script block', and finally the last one, the 'console block'.

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RStudio_4Blocks.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/RStudio_4Blocks.png?raw=true"/></a>

You may not be able to see the 'script block' on your computer for the moment, and again, this is completely normal! Just follow the steps below.

### 1.2 The computer block

<p>The 'computer block' is the one on the bottom right side. I call it the 'computer block' but it's actually much more than that, but let's keep it simple for the moment.</p>
<p>First, click on the Files button. You will see that there is a list of files and folders from your computer. This is actually the interface you can use to communicate and navigate directly with your computer! </p>

<p class="notice--info"><strong>Again, look at all the options and play with them to understand what everything's about:</strong><br> 
1/ Click on the files. How do these open? In RStudio? Directly on your computer?<br> 
2/ Try to go to other folders on your computer using the computer block. You'll see there is no mystery, this is just like navigating on your own computer as you usually do!<br></p>


### 1.3 The variable block

<p>The 'variable block' is the one on the top right side, as in the image below.</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/VariableBlock_Raw.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/VariableBlock_Raw.png?raw=true"/></a>

<p>Basically, the most important tab is the 'environment' one. This is where the variables we create when coding will be stocked. The term 'variable' can be quite abstract at the moment, so let's just exemplify it with our first code.</p>
<p>R can be used as a simple calculator. In the 'console block', just write the following code, end press 'enter':</p>

```
4+2
```
<p>Normally, you'll see this:</p>
```
> 4+2
[1] 6
```
<p>And indeed, '4 + 2' equals 6. Now, let's play a game. You want to obtain the number 8, but you have to use '4 + 2'. One option is to add 2 one more time, and you'll write the following code:</p>
```
> 4+2+2
[1] 8
```
<p>The game may continue, and you'll need to write even more. This is when the variables can be useful. Try the following code:</p>
```
a <- 4+2
```
<p>Unlike what you've seen before, nothing appears in the console anymore. But there's something new in the variable block:</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/VariableBlock_WithVariable.png?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/VariableBlock_WithVariable.png?raw=true"/></a>

<p>You stocked the calculation '4+2' as a variable, and you can call it anytime you want! For example, you can call it by simply writing `a` in the console, and you can also add 2 to it by writing `a + 2`, and you'll see something as follows:</p>

```
> a
[1] 6
> a+2
[1] 8
```
<p>This example is just here to show what the 'variables' are. With just simple calculations like the ones above, it seems to be quite useless. But you'll realize very quickly through this tutorial that variables are not only useful, but also necessary to handle more data.</p>

### 1.4 The console block
<p>Now let's talk very briefly about the 'console block'. You just had a glimpse of it when reading the section on the variable block. Actually, there's not a lot more to say about it. <strong>The console block is the place where the code is written and being run.</strong></p>
<p>In addition to the 'Console' tab, there are also the 'Terminal' tab and the 'Background Jobs' tab. Despite their importance, we won't have have to use them in this tutorial. So let's just skip them!</p>

### 1.5 The script block
<p>The 'script' block is where you'll work most of the time. You can see it as the Word or the Note Pad of RStudio. You will better understand the importance of the scripts, one more time, with an example. If you've followed Section 1.3, you can see that you have the same code as below in your console.</p>

```
> 4+2
[1] 6
> a <- 4+2
> a
[1] 6
> a+2
[1] 8
```
<p>Now, just close R and reopen it. All the codes disappeared! We usually use R for much more than a simple calculator, and we always end up with hundreds of lines of codes. Imagine if you need to rewrite everything each time you close and reopen R... and this is where the scripts are useful!</p>
<p>Let's do a simple exercise with the script. First, open a new script by clicking on "New File", and then the first option, called "R Script". </p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/OpenNewScript.gif?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/OpenNewScript.gif?raw=true"/></a>

<p>Write the lines below in the script block:</p>
```
4+2
a <- 4+2
a
a+2
```
<p>After that, select everything, and click on 'Run'. You can also have a look at the short video below.</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/Script_Demo.gif?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/Script_Demo.gif?raw=true"/></a>

<p>This is how you run a script! Alternatively, you can select everything (or just the line you interested in), and press 'enter' on your keyboard. Now you can save your script ("File > Save") and close R. Find the file you just saved on your computer and open it. Your code is still here!</p>

### Exercise: Play with your blocks!

<p>Your four blocks are like construction toys you can play with. You can make them disappear and then reappear, you can change their size as you wish, and you can even change the background color. In other words, make RStudio your own!</p>

<p>This is how you can change the size of the blocks with your mouse:</p>

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ChangeBlockSize.gif?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ChangeBlockSize.gif?raw=true"/></a>

<p>This is how you change the background color of RStudio:</p>

```
Path: Tools > Global Options... > Appearance > Choose the theme you like in 'Editor theme'
```

<a href="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ChangeColor.gif?raw=true" class="image-popup" target="_blank"><img src="https://github.com/aymeric-courses/formosan-corpus-r/blob/master/assets/images/ChangeColor.gif?raw=true"/></a>

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
