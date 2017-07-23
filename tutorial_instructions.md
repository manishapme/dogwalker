# How I built Dogwalker

This is a tutorial detailing every aspect of building a web app using Python and related convenience libraries. 

I attended a 12 week coding bootcamp at
Hackbright Academy. It was a great program, but they teach using the Flask
framework. Flask is an awesome framework, but it's really important to be able
to just write Python if you're going to take a job as an engineer. You need to
understand how to implement things yourself instead of only following a very predetermined format that a good framework has implemented.

The other purpose of this tutorial is to document all the ancillary steps that sometimes get overlooked. It is written from the perspective of a developer
using a Mac running Sierra, with a basic level of comfort around the terminal. 

## Writing Markdown

This tutorial is written in github markdown, indicated by the file ending ".md". Since many organizations document code and processes in their repos, it's important to be able to write docs in markdown. It's easy, learn by following
the [GitHub guide](https://guides.github.com/features/mastering-markdown/).

## Setup git repo

### Directory structure
I have a folder in my home directory that I call `code`. In here I have a folder
for each repo (project) that I'm working on. Open your terminal and set create
code folder if it doesn't already exist.

1. Make the parent directory
   * `cd code`
1. Make the project directory
   * `mkdir code/dogwalker`
1. Navigate into project directory
   * `cd code/dogwalker`
1. Initialize the project as something that will be archived by git
   * `git init`

### Create repo in github
1. Login to your github account and create the repo there
   1. Login to github.com
   1. Click on "repositories" from nav
   1. Click on the green "New" repo icon
   1. Enter the name of "dogwalker"
   1. Choose "public"
   1. Click "Create repository"

### Make initial commit
This next step assumes you have already setup your github account to allow
commits from your mac using ssh keys. This [Github Article](https://help.github.com/articles/connecting-to-github-with-ssh/) explains how to complete that
prerequisite.

1. From your terminal, inside the "dogwalker" directory, add a [remote](https://help.github.com/articles/adding-a-remote/) repo 
   1. `git remote add origin https://github.com/manishapme/dogwalker