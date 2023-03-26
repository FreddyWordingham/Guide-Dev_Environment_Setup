# Git - Version Control

Git is a tool for tracking changes within a directory of files.
We use it for software development because it allows us to track changes to our codebase over time.
We can also use it to collaborate with others on the same codebase by branching and merging changes.

## Installation

This triggers `macOS` to install the `Xcode Command Line Tools`, which includes `git`.

```shell
git --version
```

## Usage

Log in to your `GitHub` account:

```shell
git config --global user.name "Your Name"
git config --global user.email "your.email@domain.com"
```

Clone a repository:

```shell
git clone https://github.com/FreddyWordingham/Guide-Dev_Environment_Setup.git
cd Guide-Dev_Environment_Setup
```

Create a new branch:

```shell
git checkout -b new_branch
```

Add files to the staging area:

```shell
git add .
```

Commit changes:

```shell
git commit -m "Commit message"
```

Push changes to the remote repository:

```shell
git push origin new_branch
```

Note that you will need to have adequate permissions to push to the remote repository.

You can merge your branch into the `main` branch by creating a pull request on `GitHub`.

## Return

[Return to the top-level README](./../../README.md)
