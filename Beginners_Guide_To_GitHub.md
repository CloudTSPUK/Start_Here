##Introduction
The purpose of this guide is to provide an introduction to the core workflow associated with leveraging GitHub as a version control system. 

This particular guide illustrates a browser based workflow for interfacing with the GitHub website to achieve basic **[Git](https://help.github.com/articles/github-glossary#Git)** tasks. Being based on GitHub this guide does not leverage any specific local Git client(s). A Git client is used to interface with a Git version control server to retrieve, manage, track and eventually sync local repositories and file changes back to a Git server.

**The core workflow/principles outlined in this guide apply irrespective of whether you are directly interfacing with online Git servers such as GitHub or Visual Studio Team Services or if you are working offline via Git clients that interface with GitHub, Visual Studio Team Services or other Git based version control systems.**

Some of the dedicated Git clients include:
* [GitHub for Desktop]( https://desktop.github.com/) application.
* [Visual Studio’s GitHub Extension]( https://visualstudio.github.com/) providing integrated Visual Studio tooling for GitHub. 
* [Git Command Line Interface](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

This guide visualises and, where appropriate, builds upon the official introductory GitHub Hello World guide found [here](https://guides.github.com/activities/hello-world/).

This guide assumes you have GitHub.com account and Internet access, this is all that is needed to complete this guide. 

### 1. Log into [GitHub](https://github.com/)

### 2. Create a new [Repository](https://help.github.com/articles/github-glossary#repository)
The first step to creating any project or body of work when using Git is to create a new repository. 

Respositories can be created as being either Public or Private. 
* A Public repository is a repository that is discoverable and accessible by the entire GitHub community. 
* A Private repository is a repository that is not discoverable by the larger GitHub community. Induvidual users need to be given direct access to the repository in order to work with it. 

The process for creating a public repository with a README file in GitHub is as follows:

![alt text](https://github.com/CloudTSPUK/Start_Here/blob/master/assets/Step_1_Create_Repository.gif "Create a repository")

### 3. Create a [Branch](https://help.github.com/articles/github-glossary#branch)
As referenced in the official glossary a branch is a parallel version of a repository. This parallel verison represents a complete copy of a repository at the point in which the branch was created.

In almost all version control systems the first branch of a project is taken from what can be refered to as the master or trunk version of the source code/project items under source control. 

Subsequent branches can be made to either the master or indeed other branches. The motivation for creating a branch and the point in time in which a branch is taken will come down to either personal preference or a wider branching team or organisation agreed branching strategy.

Some guidance on branching strategies can be found [here](https://msdn.microsoft.com/en-us/library/bb668955.aspx) and [here](https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows).

This guide will create a branch from the master of the new repository created above. A change wil then be made in this branch and not on the master.

![alt text](https://github.com/CloudTSPUK/Start_Here/blob/master/assets/Step_2_Create_A_Branch.gif "Create a branch")

### 4. Make and [commit](https://help.github.com/articles/github-glossary#commit) changes
Changes occur as you edit and update a file that is under source control. In this guide the only file currently under source control is README. 

Below illustrates the process for editing the README file in browser and then committing this file with its changes to (in this instance) GitHub. It is considered good practice to provide some commentary or insight into the motivation for a change that is to be commited. 

![alt text](https://github.com/CloudTSPUK/Start_Here/blob/master/assets/Step_3_Make_and_commit_changes.gif "Make and commit changes")

### 5. Open a [Pull Request](https://help.github.com/articles/github-glossary#pull-request)
Comitting a change to a branch in a repository on GitHub does not immediately guarantee that a change is accepted into the master of that repository. 

In order for a committed change to be included into the master (or branch) of a repository a commit must be associated with a Pull Request. 

Creating a Pull Request can be thought of as creating an indicator to the owner of the of the branch informing them that a change or contribution has been made that can be reviewed and considered for inclusion in the branch. 

The process for creating a Pull Request is demonstrated below.

![alt text](https://github.com/CloudTSPUK/Start_Here/blob/master/assets/Step_4_Open_a_Pull_Request.gif "Open a Pull Request")

A further breakdown of a typical Pull Request can be seen below.

![alt text](https://github.com/CloudTSPUK/Start_Here/blob/master/assets/Anatomy_Of_A_Pull_Request.PNG "Anatomy of a Pull Request")

### 6. [Merge](https://help.github.com/articles/github-glossary#merge) your Pull Request
![alt text](https://github.com/CloudTSPUK/Start_Here/blob/master/assets/Step_5_Merge_your_Pull _Request.gif "Merge a Pull Request")

**Note**: This guide illustrates an example of where a single user is working in a purely online capacity. This is an example of where the author of the commit and the creator of the pull request owns both the branch and the master of the repository. Due to this the process of creating a pull request for a commit on a branch only to accept and merge said pull request back into the master can appear as slightly convoluted and potentially redundant. 

This example can lead to the question **"Why should I even bother to create a branch when I can simply edit the master directly?"** 

It is generally accepted that branches offer a mechanism for handling different variations of the same application or project code base. These variations will come about as a result of iterating or changing the product/master source code. It could be that each new iteration of the product or each new proposed feature of the product could reside in its own branch. 

It would then be a further consideration as to whether to keep all of these branches or to merge them back into either a parent branch or indeed the master source code. 

All of these types of considerations will come down to the projects broader [branching strategy](https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows).

