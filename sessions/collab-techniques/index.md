---
layout: session
title: Software engineering techniques for collaborative software development
instructor: David Luet
---

This session builds on the previous one on Version Control with Git and GitHub to introduce important concepts of collaborative software development.

We will start by introducing Git concepts that relevant when we work as part of a team. Then we will see how developing test suites is an essential part of programming, even when we work on your own, and is crucial when working collaboratively.

Within a team of developers if one developer's changes break the code, this will impact everyone's work. Regression testing—that is; making sure that the old functionalities are still valid—will protect you against lost of productivity and potential embarrassment.

By testing code modifications automatically, with tools like Travis or Jenkins, you maximize your chances of catching errors before they are added to the shared code repository.

This idea of automatically testing every changes to the shared repository is part of a software engineering practice called Continuous Integration (CI). This session is about adapting CI principles to the practice of scientific software development.
