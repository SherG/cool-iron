---
title: How to Create a Pull Request in Github
path: /pull-requests
date: 2022-05-28
summary: Here's an easy cheat sheet for making pull requests in Github.
tags: ['code', 'websites', 'tutorials']
---

I use Github fairly often, but rarely make pull requests. When I go to create a new one, I find I need a refresher on how to do it. 

So I decided to create this short cheatsheet for myself. Perhaps you'll find it helpful as well. 


## What is a pull request? 

A pull request is a technique for suggesting edits to someone's code base. Like the "review suggested edits" feature in Google Docs, a pull request provides the code repository owner with an easy way to review your suggested edits and incorporate them into their code if they wish.

### Reasons for making pull requests 

Some reasons for making pull requests include: 

* You're a newbie coder who wants to start contributing to existing projects
* You noticed an error and would like to propose a fix
* You'd like to solve an existing problem discussed in an Issues thread on the repository.
* You'd like to propose an improvement: such as a more efficient way of executing a task. 

## How do you create a pull request? 

1. Fork the original repository. (A fork is a copy of someone else's code that you can edit.)

2. In the forked copy, navigate to the page that you want to alter.

<img src="https://res.cloudinary.com/icecloud7/image/upload/f_auto/v1653749339/SignalFox/github-pull-request-page_ijysu7.png">

In the example above, I nagivated to the /layouts/partials/categories.html page. My goal is to correct a code typo: I want to remove the brackets highlighted in yellow. 

3. Click the edit button, edit the code, then save. 

4. Click on "Pull requests" near top left

<img src="https://res.cloudinary.com/icecloud7/image/upload/f_auto/v1653749340/SignalFox/github-pull-requests-button_ieoino.png">


5. Now you'll see your code suggestion (highlighted in green) below the original code (highlighted in red). Check to make sure your code is correct. Then click the green "Pull request" button at upper right. 

<img src="https://res.cloudinary.com/icecloud7/image/upload/f_auto/v1653749342/SignalFox/pull-request-code-comparison_ivr4se.png">

You'll have a space to briefly explain your proposed change.

The code repository owner will be notified. Once he or she reviews your code suggestion, and acts on it, you'll be notified. 

In the case used in the example, the repository owner accepted the suggestion and <a href="https://github.com/zwbetz-gh/minimal-bootstrap-hugo-theme/pull/21/commits/fc0fa96451eae545d193cb9b845a21fc52240bd7" target="blank">merged</a> the code. 

Fun fact: if your code suggestion is accepted, you are now a contributor to their code project. Your contribution will be documented on their page and your profile photo will appear as a contributor. 

### Q&A 

Have more questions? Drop me an email or peruse these QAs.

#### How do you fork a Github repository? 

To fork a Github repository navigate to the repository page, then click the "fork" button at upper right. The forked copy will now appear in your account under "Your repositories." 

#### I'm a newbie: how do I find ideas for pull requests? 

On a repository page, go to the "Issues" tab, then click "Labels." Click on "good first issue" (described as "good for newcomers.") Try choosing an active repository of a popular, but simple template, built with a site builder you're familiar with, such as Hugo, Jekyll, or Skeleventy.

### More tutorials 

<a href="/optimize-images-cloudinary" target="blank">How to use Cloudinary to optimize images</a><br/>
Optimizing your images is one of the most powerful solutions to poor loading speed. You only need a beginner's knowledge of HTML to use this tutorial.

<a href="https://www.signalfox.org/optimize-images" target="blank">How to optimize images for the web</a><br/>
Your website has an obesity problem. Here's an overview of your options for trimming those enormous images down and delivering a better experience for your users.
