---
layout: post
title:  "Understanding Git and Github"
comments: true
categories: git
date: 2020-12-02 16:38:20
i: true
img: https://github.githubassets.com/images/modules/open_graph/github-mark.png
k: true
---

Git is a open source version control system. Basically it's a software where we can manage and build the different versions of our software. It is a distributed service that contains history, edits, updates of the files.  GitHub on the other hand is a repository hosting service which is like a server that contains all our files and has git software installed on it.
<!--
Still difficult? Ok lets take an example why git is used and what makes it an integral part of the IT community. The typical software cycle involves a lot of steps like development, deployment, testing etc involving a large number of people working in collaboration. -->

In this article we'll dive into two methods to initiate and work on a project locally and how to connect it remotely to a repository hosting service like GitHub or bit-bucket.

---

The first method is by cloning an existing repo on github or any other hosting sote.

``` bash
  git clone https://examplerepo.org/something.git #creates a empty git repository in your local server
```
This will create a copy of a repo on your local pc where you can start changing the files.
Once we have done necessary changes and our files are ready we can add it back online using following commands.
``` bash
  git add . #adds all the files to the local index
  git commit -m "any comment here"
  git push origin master # to push the changes to the master branch
```
---
The  second method is to intitialize an emtpy git repo and then create a link online to github repo.
This can be done by
``` bash
  git init # create an empty repo
  git echo "# hello world" > readme.md # create a readme files
  git add . # adds into local
  git remote add origin https://examplerepo.org/something.git
  git push --set-upstream origin master
```
This will push all the files to the master branch of the repository hosted online.

We can create a branch and push the changes as follows:
``` bash
  git checkout -b brache1 # created a branch from master
  git remote add origin https://examplerepo.org/something.git
  git push --set-upstream origin branch1
```


Here are few links to understand this topic in further detail:
- [Roger Dudler's guide](https://rogerdudler.github.io/git-guide/)
- [GitHub's official guide](https://guides.github.com/activities/hello-world/)
