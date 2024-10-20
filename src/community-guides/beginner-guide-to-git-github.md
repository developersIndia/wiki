# Beginner Guide to Git And GitHub

## Introduction to Git and GitHub

Git and GitHub are two essential tools for a developer when it comes to version control and collaboration. In this section, we'll look into the unique functionality of both software and identify their differences.

## Difference between Git and GitHub

## Git

Git is an open-source, command-line-based **version control system** (or time machine) developed by Linus Torvalds in 2005 with regard to develop a Distributed Version Control System which is ***fast,reliable and support non-linear development.***

It is installed, lets you manage and **keep track of your source code history locally.** However, the main feature of Git is its branching model. Git lets you create independent branches in your code and allows you to try out new ideas, reroll back to earlier versions, delete and merge branches, etc. It also enables collaboration by allowing multiple developers to work on the same project simultaneously, without stepping on each other's toes.

## GitHub

GitHub is a **Git repository hosting service** owned by Microsoft Corp. Basically, it provides a platform to store and manage Git repositories online. Unlike Git, GitHub is entirely cloud-based and proprietary software. GitHub expands on Git's functionality. It has a web-based interface and built-in functions for issue tracking, pull requests, code review etc. Its ability to share code online and facilitate collaboration makes it a popular social coding platform.

Here's an analogy: Think of Git as your recipe book, where you can meticulously track every tweak and variation of your favourite dishes. GitHub is a giant online cookbook community where you can store your recipes, share, discover new ones and cook up amazing meals together.

The wording you've used is mostly appropriate, but there are a few adjustments that can make the explanation more precise and aligned with Git terminology:

### Three States/Stages in Git (Basic Workflow)

> Before understanding the three stages in Git, it's important to know that all the information about changes to your project is stored inside the **.git directory**, which gets created when you initialize a project or folder to be version controlled by Git. **This .git directory functions as a local database, storing the entire history of the project.**

1. **Working Directory**: This is where you make changes to your source code—it's your active project directory where files are created, edited, or deleted.

2. **Staging Area (Index)**: This is an intermediate layer between the working directory and the repository. Here, changes are prepared for the next commit. You add files to the staging area to mark them for inclusion in the next commit.

3. **Repository (.git directory)**: This is where commits are stored as snapshots of the project. When you commit, a snapshot of the files in the staging area is saved in the repository. Unlike some other version control systems, Git creates a snapshot of the project's entire state, but it efficiently stores only the changes between commits.

> **Note:** While Git takes a snapshot of the entire project at each commit, it stores changes efficiently by saving only the differences between files. This approach differs from some other version control systems, which may store only the modified files.

## F.A.Q

Q. What do you mean by version control systems and how do they help us?

>Version control systems(**V.C.S**) are a piece of software to track changes done on some file or source code that we want to.

V.C.S help us in various ways :

1. Manage changes/versions of our file.
2. Act as a backup for history of our project/source code.
3. Revert changes done if something unforseen happens due to present code.

Q. Difference between Local, Central and Distributed V.C.S?

In early times people used to manage different versions of their projects locally using different folders for each versions. This was called local version management

Disadvantages of local version management

1. Inability to share the source code with others.
2. Hard maintenence of the project.

To tackle with the disadvantages of the local version management **Central V.C.S** came into picture.

Central V.C.S stored the project over to a **central repository** and was made accessible to all the different clients working on the project.

Example : Perforce and CVS.

Disadvantages of Central V.C.S

1. Had a network latency involved while working on the project.
2. The project being allocated at a central working directory was prone to damages and data loss.

To solve the major problems in both local and central V.C.S
Distributed Version Control Systems were developed which handled the problem of centralness of CVCS by distributing copy of the project to entire repository to each of the client.

Q. How is git different from other Version control systems?

Git is different from other version control systems because of its nature to create snapshots of the entire project instead of only tracking changes (often known as **delta changes**) to the particular files.

<!-- # Resources -->
