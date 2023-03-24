# Homebrew - Package Manager

A package manager will allow us to install and manage software packages from the command line.
Homebrew (`brew`) is a package manager for `macOS`.
It is similar to `apt` on `Ubuntu` and `yum` on `CentOS`.
These tools allow us to install, update, and uninstall software packages and dependencies.

Once we have installed `brew`, we'll use it to install the other software we need to set up our development environment.
While we could execute a raw shell script (like we're about to do here using `curl`) it is not recommended because it is far less secure.

## Installation

Navigate to https://brew.sh and copy the code into your terminal to install `brew`:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Then add the `brew` command to your `PATH`:

```bash
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/freddy/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Usage

To install a package, run the following command:

```bash
brew install some_package_name
```

To install a graphical application, run the following command:

```bash
brew install --cask some_app_name
```

To update all installed packages, run the following command:

```bash
brew upgrade
```

To uninstall a package, run the following command:

```bash
brew uninstall some_package
```

## Details

Homebrew (`brew`) is a popular package manager for `macOS` that allows users to easily install and manage a variety of software packages, libraries, and utilities on their machines.

With `brew`, users can install, update, and uninstall software packages and dependencies from the command line, without the need for manual downloading, compiling, or configuration.
Homebrew uses a formula system, where packages are defined as "formulae" in `Ruby` scripts, which are then downloaded, built, and installed from source code or precompiled binaries.

Homebrew also allows users to create and maintain their own formulae, contribute to the community-maintained repository of formulae, and use "casks" to install graphical applications and other binary packages.
It provides a convenient and streamlined way for developers and users to manage the software dependencies and tools needed for their projects or workflows.
