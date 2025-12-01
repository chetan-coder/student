---
toc: false 
layout: post
title: Tools Journey 
description: Journey with development tools -- GitHub, Cloning, Virtual Environments, and Running a local website.
permalink: /tools/journey
---

## Visual Journey

Linux is the most compatible OS for Developers. 

This visual help remind me of Tools and their relationship to my Development Journey. 

Step 1: Create Accounts
First thing I did was make a GitHub account to store my code and a Slack account to communicate with my class. I learned pretty quickly that I need to be careful about what personal info I share online - protecting PII is super important.

Step 2: Set Up macOS
Since I'm on a Mac, I got familiar with Terminal. It's basically where I run all my commands to set up projects and manage code. macOS works really well for development tools, which made things easier.

![Setup MacOS Termonal]({{site.baseurl}}/images/commits.png)

Step 3: Install Tools
I downloaded VS Code as my main code editor - it's where I actually write all my code. Then I installed Git for version control so I can track changes and push my work to GitHub. I also set up Python, Jupyter Notebooks, and other packages I need for my projects.

Step 4: GitHub Repositories
I forked the student template repository to create my own student repo. This is where all my personal projects live. I also cloned the class pages repository just as a reference to look at when I need help.

![Forked Student Repository]({{site.baseurl}}/images/repositories.png)

Step 5: Clone to Local Computer
I cloned both repositories to my Mac so I could work on them locally. They're organized in my documents folder where I can easily access them.

Step 6: Virtual Environment Setup
For each project, I run ./scripts/venv.sh to create a virtual environment, then source venv/bin/activate to activate it. This keeps all my project dependencies separate and organized. After that, I type code . to open everything in VS Code.

Step 7: Development Workflow
Now I can actually code! I write my code in VS Code, test it, and debug any issues. When I'm done, I use git add and git commit to save my changes, then git push to send everything to GitHub.

Step 8: GitHub Pages
The cool part is that GitHub automatically deploys my website whenever I push changes. So my code goes live on GitHub Pages and I have a real portfolio website that anyone can visit.

Step 9: Troubleshooting
When things break (and they do), I use the pages repository as a reference to see how things should work. I've learned common commands and how to fix typical issues that come up during development.

This image shows the commits I've done after achieving all of these steps.

![Commits]({{site.baseurl}}/images/commits.png)
