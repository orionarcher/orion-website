---
title: "Ode to Cookiecutters"
tags: ["GSoC", "Molecular Dynamics", "Message"]
description: "A few thoughts on the MolSSI cookiecutter."
author: "Orion Cohen"
date: "2020-07-21"
---

If my only takeaway from Google Summer of Code was how to download and setup the [MolSSI cookiecutter template](https://github.com/MolSSI/cookiecutter-cms), I would still consider it a success. Before this summer, I knew in my heart that I should be using tools like version control and continuous integration. I knew testing would make my code easier to extend and that documentation would make my code easier to understand. Nonetheless, amidst the tumultuous reality of academic life, I rarely found the time to implement any of these practices, let alone all of them. I falsely believed that it would a lot of time and energy to set them up, when in reality, tools like [cookiecutter](https://github.com/cookiecutter/cookiecutter) make it incredibly easy.

The MolSSI cookiecutter template automatically constructs a GitHub repository with best practices built in. I won't write a full feature list, but it includes pre-built documentation, GitHub hooks for continuous integration, preconfigured `setup.py`, a skeletal directory structure, and more. With a few hours of effort, I was able to get a fully featured GitHub repo up and running. In other words, I was able to eliminate a main barrier to reproducible research in a matter of hours. In this blog post, at the risk of sounding like a laudatory scientific infomercial (call 1-800-555-4890 to get your MolSSI template now!), I'll outline a few concrete ways the template has improved my development workflow. 

### 1. Organizing my Code

A few empty folders can be surprisingly impactful. The MolSSI default directory structure is relatively simple, but it provides folders for code, data, and tests. It also puts `__init__.py` files in the right places to create a package structure, letting me import functions with absolute imports rather than any hacky solutions with file paths. Even though this was simple to set up, I hadn't done it before. The real secret of the MoLSSI template is that it does many easy things for you.

### 2. Easy Feedback

Abundant and incredibly helpful feedback has been the defining feature of my GSoC experience. My mentors have helped me with everything from program structure to typos in the documentation. Without GitHub issue tracking and pull requests, that sort of feedback would be impossible. While a cookiecutter obviously isn't a prerequisite for using GitHub, it's worth noting that a lot of scientific code exists outside of version control entirely, floating in the ether or Dropbox or Google Drive. Having a template force me onto version control has been a good thing.

### 3. Scaffolding for Testing

Basic continuous integration and testing with [pytest](https://docs.pytest.org/en/6.2.x/) is backed up with code coverage results from [codecov](https://about.codecov.io/). After I write tests, codecov visually displays what I missed and continuous integration ensures my code works across python versions and operating systems. These advantages are most apparent when I need to refactor code. In the past, refactoring always involved a lot of hand wringing because I'd worry that my changes would break some functionality. Now, I just rerun all the tests and I am confident that my code still works.


### 4. Fodder for Prosthylatizing

Ok, admittedly this isn't an improvement to my development workflow but it is nonetheless a core advantage to me personally. I, like many scientists, am concerned about the growing "[reproducibility crisis](https://www.nature.com/articles/s43588-021-00109-9)" in scientific software. Put simply, most scientific code isn't really reproducible because it lacks testing, documentation, and many of the other features I've mentioned. Busy scientists don't implement these practices because they don't know how and they feel like they don't have time. It's hard to convince a researcher that it is worth a big time investment to learn to become a better software engineer. That's where templates like this can really help, by allowing busy scientists to easily make their research code more reproducible. In the future, when I try to sell my friends and colleagues on software best practices, I look forward to pointing to the MolSSI template and saying, "here, this is where you get started."