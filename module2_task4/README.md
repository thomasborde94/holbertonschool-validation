<h1 align="center"> Module 1: Introduction to DevOps: Automate Everything to Focus on What Really Matters

# Learning Objectives
This project aims at showing use cases where a DevOps mindset is bringing value to a software project by automating it, which decreases the amount of manual work and increases the development speed. It focuses on why automation is useful and helps speeding a development lifecycle.

After this project, you should be able to:

- Understand the value of automating tedious tasks
- Define a development lifecycle
- Automate shell-like tasks with Make, and/or shell script
- Be aware of tools dependencies and the value of reproducing environment
- Build static HTML website from Markdown code using Go-Hugo

## Prerequisites

The following elements are required:

### Concepts

You should have a basic knowledge of the following concepts:

- Shell terminal basics, using command lines:

	- Navigating in a Unix file-system
	- Understanding how stdin/stdout redirection and piping
	- Showing and searching the content of a text files
	- Defining and using Environment Variables
	- Adding command lines to your terminal using the apt-get package manager and/or with the PATH variable
	- Writing and executing a shell script

- Git with the command line (and also a graphical interface)

	- Retrieving or creating a repository
	- Manipulating changes locally with Git’s 3 steps process (workspace, staging, history)
	- Distributing changes history with remotes repositories

- Make/Makefile usage:

	- Executing tasks through make targets
	- Default target and PHONY target
	- Makefile’s variables and macro syntax

### Tooling

This project needs the following tools / services:

- An HTML5-compliant web browser (Firefox, Chrome, Opera, Safari, Edge, etc.)
- A free account on [GitHub](https://github.com/), referenced as `GitHub Handle`
- A shell terminal with bash, zsh or ksh, including the standard Unix toolset (ls, cd, etc.)
- [GNU](https://www.gnu.org/software/make/) Make in version 3.81+
- [Git](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line) (command line) in version 2+
- [Go Hugo](https://gohugo.io/) v0.84+
- [markdownlint-cli](https://intranet.hbtn.io/rltoken/hplwMW8M8BKVQyhDso0pOw) v0.26.0
- [markdown-link-check](https://intranet.hbtn.io/rltoken/BRJGBHXvkAUKt50KrFOm0A) v3.8.6
- [Holberton's W3C Validator](https://intranet.hbtn.io/rltoken/ll8gJ8CPoI9tfn1OTDE8rA)


<h1 align="center"> How to use the make file:

## Lifecycle

In the DevOps methodology, the development lifecycle is generally staying the same. Use the following steps :

To execute the Makefile use the following syntax:
 ```make <command>```

4 command are availaible :
 `make help`:
    - show all command description

 `build`:
    - Builds a new version of the website to folder `/dist/` 

 `clean`:
    - Removes the contents the folder  `/dist/`

 `post`:
    - Creates a new post in the contents/post folder with POST_TITLE and POST_NAME set from the ENV variables.

 `check`:
	- Lint of the Markdown source files using command line AND analysis of the links with command line. If one test fails, the command failed.
 
 `validate`:
	- validate the file ./dist/index.html by using command line. But non-blocking quality indicator


# Story
Congratulations!

It’s your first day at “Awesome Inc.” as a software engineer. This company is currently experiencing fast growth and hired you to work on their web services.

Your predecessor left to travel the world, and the expectations are high on your ability to help "Awesome Inc.” to grow a culture of collaboration with a technical mindset, while managing their existing web services. That’s exactly what DevOps is about!