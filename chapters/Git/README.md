# Git - Version Control

`git` is a tool for tracking changes in any set of files.

## Installation

This triggers `macOS` to install the `Xcode Command Line Tools`, which includes `git`.

```bash
git --version
```

## Usage

Log in to your `GitHub` account:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@domain.com"
```

Clone a repository:

```bash
git clone https://github.com/FreddyWordingham/Guide-Dev_Environment_Setup.git
cd Guide-Dev_Environment_Setup
```

Create a new branch:

```bash
git checkout -b new_branch
```

Add files to the staging area:

```bash
git add .
```

Commit changes:

```bash
git commit -m "Commit message"
```

Push changes to the remote repository:

```bash
git push origin new_branch
```

Note that you will need to have adequate permissions to push to the remote repository.

## Details

Software is not written in a single sitting, it grows and evolves over time.
It is unlikely that the final architecture of a software system will be known at the start of a project because we'll always encounter hurdles and unexpected problems along the way.
Prototypes and experimentation should be how we approach a perfect solution, not pure theory.

So to reach a well-architected result we are **going** to meander through several different experimental approaches.
And what's more is that they are unlikely going to be monotonically better than the previous one.
For this reason, it is important to be able to track changes to the codebase over time and to be able to revert to previous versions if necessary.

Version control is the management of changes to a file or set of files over time.
It is a system that allows developers to track and manage changes to their code, collaborate with others, and maintain a history of their work.

A version control system (VCS) allows developers to keep track of changes made to a file or set of files over time. It can track who made changes, what changes were made when they were made, and why they were made.
This is useful when multiple developers are working on the same codebase, or when a developer needs to make changes to an existing codebase without losing the original code.

There are several popular version control systems, including [`git`](https://git-scm.com/), [Subversion](https://subversion.apache.org/) (`svn`), and [`mercurial`](https://www.mercurial-scm.org/wiki/HgSubversion).
These systems typically offer features such as branching, merging, and tagging, which allow developers to work on different versions of the same codebase simultaneously, merge changes from different branches, and label specific versions for release.
