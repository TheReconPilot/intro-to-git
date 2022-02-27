# Git
\- Purva, IPLUG

## Introduction

You must have seen, and probably done something like this yourself:

- Report.docx
- Report-Final.docx
- Report-FinalChanged.docx
- Report-FinalFinal.docx
- Report-Final3.docx
- Report-TheUltimateFinal.docx

Whenever we work on something, it's usually not a job finished in a single sitting. There are changes, additions and deletions. Don't you sometimes wish you could go back to how your work was at a specific point when the Undo button isn't available anymore?



That's where **Version Control Systems** (VCS) come in. A VCS saves your work at different moments, so that you can go back to some point in the past. If you have ever used the History feature in Google Docs, it is similar to that.



Git, Mercurial, SVN are some examples of Version Control Systems which are primarily used for code, but can be used for just about any work. We will be talking about Git, the most popular VCS.



## What is Git?



- Git is a VCS.
- It snapshots your work at any given moment that you want it, along with a helpful **commit** message.
- A folder can be initialized to work with Git. Such a folder is called a **Repository**. It is called *Repo* in short.
- You can have Git store your repos at some remote place.



### Git vs GitHub



GitHub is like a Google Drive for Git Repositories. GitHub allows you to store any repos that are initialized with Git. It acts as a remote place to store your work.



The primary benefit is that it makes **collaboration** easier and much more feasible. Imagine many people working on a codebase, of course, they can't work on a single computer on a single local folder. Here's where the power of Git as a VCS and GitHub as a storage medium comes in.



## Git Basics



### The Idea



- We initialize a folder as a *Git Repository*. This folder is also our **working directory**. 
  - The working directory is our live working folder, just a simple folder in the normal sense.
  - The repository is where git stores snapshots of the work.
  - In practice, we call the folder both a repo and a working directory.
    
- Whenever we do some little work that we feel should be saved, we **add the file(s) to the staging area** and **commit** with a helpful message.
  
- Git stores a snapshot of the folder with the commit message and a unique id (an SHA256 hash).



![](https://geo-python.github.io/site/_images/Git_illustration.png)



Image Source: [Git Basics, Geo Python, University of Helsinki](https://geo-python.github.io/site/lessons/L2/git-basics.html)



- We can also have our work sync with some remote repository or backup. That could be present on any services like GitHub, GitLab, etc. 
  - We can **push** any changes on our local repo to the remote repo.
  - We can **pull** any changes from the remote repo to our local repo.
    
- We can **revert** any changes at a later time.
  



 

![](https://geo-python.github.io/site/_images/pull-push-illustration.png)



Image Source: [Git Basics, Geo Python, University of Helsinki](https://geo-python.github.io/site/lessons/L2/git-basics.html)





- The snapshots and commits are stored in a Graph Tree like structure. The main tree is simply called **main** or **master** branch.
  
  
- We can also work on different things using the feature of **branches**. Essentially, we work on something alongside the main/master branch and we can merge changes to the main/master branch later on.

- How does Git know what branch is it on? There is always a pointer, called the **HEAD**, pointing to the latest commit on the branch we are working on.



![](https://wac-cdn.atlassian.com/dam/jcr:a905ddfd-973a-452a-a4ae-f1dd65430027/01%20Git%20branch.svg?cdnVersion=233)



Image Source: [Using Git Branches, Atlassian](https://www.atlassian.com/git/tutorials/using-branches)





![](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)



Image Source: [Git Branches, Noble Desktop](https://www.nobledesktop.com/learn/git/git-branches)

