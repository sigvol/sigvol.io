---
title: 'A workflow for Git and GitHub'
date: 2018-09-09
permalink: /posts/2018/09/blog-post-2/
tags:
  - MII
  - GitHub
  - tutorial
---
This is a [re-blog](http://www.matiasz.com/2015/06/30/a-workflow-for-git-and-github/) from my 
labmates [NICHOLAS J. MATIASZ](http://www.matiasz.com/2015/06/30/a-workflow-for-git-and-github/).
It aims to help people get familiar with Git and GitHub workflow.

Although version control is useful for all software development, 
team-based development particularly highlights the need for tools like Git and GitHub. 
Team-based development can get complicated, though, when each teammate has unique 
preferences for version control tools and workflows. In this post, 
I present the Git/GitHub workflow that I currently use, and I share my impressions from 
using it daily. In my experience, this workflow offers a sweet spot with respect to the 
time it requires and the benefit it delivers. This workflow makes me more productive, 
and—when done right—it blurs the line between version control and project management. 
Essential parts of developers’ work, version control tools and workflows should be included 
in all computer science curricula.

## Git/GitHub workflow
1. On GitHub, create an [*issue*](https://guides.github.com/features/issues/) (e.g., #17) for a specific feature, bugfix, etc.
2. ```$ git checkout master```
3. ```$ git pull```
4. ```$ git checkout -b <branch_name>``` (e.g., 17_fix_login_form )
5. Commit code with [*descriptive commit messages*](https://chris.beams.io/posts/git-commit/).
6. ```$ git push origin <branch_name>```
7. On GitHub, create a [*pull request*](https://help.github.com/articles/about-pull-requests/).
8. In the pull request’s description, write “Resolves #<issue_number>.”
9. On GitHub, [*merge*](https://help.github.com/articles/merging-a-pull-request/) the pull request.

### Notes
This workflow improves some psychological aspects of programming. 
By creating an issue on GitHub before you start to code, you are forced to 
articulate every planned task—an absolute requirement for technical work. 
As one benefit of this strategy, when you create an issue, you define a 
clear scope for your work. Defining a clear scope helps you to avoid straying 
from your goal while you code. As I navigate through a repository, 
I’m sometimes guilty of thinking, “Oh, hey—that’s broken, too.” A few minutes 
later, I’m changing some CSS when I originally intended to fix a database query. 
Before writing any code, you also benefit from describing your plan in words. 
If you can’t explain what you’re doing in plain language, you shouldn’t start 
to code.

To help you convey your ideas, GitHub’s interface allows you to paste images 
and code snippets into each description box. I often use this feature because 
a picture or code snippet will sometimes remind me of a task faster than words 
alone. Github’s text fields can also parse [*GitHub Flavored Markdown*](https://help.github.com/categories/writing-on-github/), a simple 
syntax for styling your text (e.g., with bold or italics).

Note that I like to start each branch name with its corresponding issue’s number. 
This way, I immediately know every branch’s goal, even if I haven’t worked on 
it for a while. Similarly, writing “Resolves #<issue_number>” in each pull 
request’s description explicitly ties the pull request to its issue. This latter
 method has a convenient side effect: GitHub will [*automatically close*](https://blog.github.com/2013-05-14-closing-issues-via-pull-requests/) the 
 issue once you merge the pull request.

Following this workflow yields an elaborate history of your development activity. 
Such a history removes part of the burden of having to remember where everything
 is in your codebase. Here’s an example: One of my projects uses JavaScript 
 for zooming on an SVG element in HTML. Some time ago, I created a branch and 
 pull request to adjust the minimum and maximum levels of zoom allowed for this 
 element. If, months or even years later, I want to change these zoom levels, 
 I don’t have to spend time figuring out how I first did it. I can just search 
 my repository with the term “zoom,” and GitHub will direct me to the exact 
 commit that recorded the change. GitHub’s intuitive visualizations of changes 
 between commits will even direct me to the exact line(s) of the file that 
 I changed. This situation happens frequently; my workflow helps me to avoid 
 the frustration of solving the same problem twice.

Now that I’ve used this workflow for a while, it feels taboo for me to switch 
to a new task on an existing branch. I prefer not to muddy my commit logs. 
If I want to switch tasks, I need to create a new branch. But I can’t name 
my branch until I know the issue number. And I won’t know the issue number 
until I create an issue. For those (hopefully fleeting) moments of laziness 
that developers know well, motivation is built right into this workflow. 
To follow it is to perform hygienic version control techniques.
