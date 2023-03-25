# Oh My Zsh - Shell Manager

Oh My Zsh is a framework for managing the configuration of the `ZSH` shell, providing a variety of themes, plugins, and customization options that make it easy for users to enhance and customize their shell experience.

## Installation

Visit https://ohmyz.sh and copy the code into your terminal to install Oh My Zsh.
It will look like the following:

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

When you want to add things to your `ZSH` shell start-up script, you can do so by adding them to your `~/.zprofile` file.
For example, add a greeting to your `ZSH` shell start-up script:

```shell
echo "echo 'Hello, World!'" >> ~/.zprofile
```

## Setup

### Theme

Oh My Zsh includes a variety of themes that can be used to customize the appearance of the shell, including the prompt, text colors, and more.
You can see what the themes look like at https://github.com/ohmyzsh/ohmyzsh/wiki/Themes.
Or see a list of them in the terminal by running the following command:

```shell
ls ~/.oh-my-zsh/themes
```

To change the theme, open the `~/.zshrc` file and change the `ZSH_THEME` variable to the name of the theme you want to use:

```shell
open ~/.zshrc
```

Edit the file (we'll install a text editor soon!) and change the `ZSH_THEME` variable to the name of the theme you want to use:

```shell
ZSH_THEME="robbyrussell"
```

### Plugins

The plugins for Oh My Zsh are located in the `~/.oh-my-zsh/plugins` directory, we just need to enable the ones we want to use.
We can do this by editing the `~/.zshrc` file:

```shell
open ~/.zshrc
```

And adding the plugins we want to use to the `plugins` array:

```shell
plugins=(copybuffer copyfile copypath dirhistory git jsontools macos web-search zsh-autosuggestions zsh-syntax-highlighting)
```

We'll go over each of these suggested plugins in more detail below.

#### Copy terminal buffer

The [`copybuffer`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/copybuffer) plugin adds a useful function for copying the current command buffer to the clipboard, making it easy to paste the command into other applications.

```shell
copybuffer
```

#### Copy file contents

The [`copyfile`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/copyfile) plugin adds a useful function for copying the current file path to the clipboard, making it easy to paste the path into other applications.

```shell
copyfile README.md
```

#### Copy the current directory path

The [`copypath`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/copypath) plugin adds a useful function for copying the current directory path to the clipboard, making it easy to paste the path into other applications.

```shell
copydir
```

#### Directory history

The [`dirhistory`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/dirhistory) plugin adds a useful function for navigating to a previously visited directory, making it easy to quickly jump to a directory you've visited recently.

```shell
dirhistory
```

#### Git

This plugin adds Git integration to the shell, providing useful shortcuts and prompts for working with Git repositories.

#### JSON tools

The [`jsontools`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/jsontools) plugin adds a variety of useful functions for working with JSON data, including functions for formatting, validating, and converting JSON data.

For example, to check if a file contains valid JSON data, you can use the `is_json` function:

```shell
is_json < data.json
```

#### MacOS aliases

The [`macos`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/macos) plugin adds a variety of useful aliases and functions for working with macOS, including shortcuts for common commands, such as `ls`, `grep`, and `find`.

```shell
ls
```

#### Web search

The [`web-search`](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/web-search) plugin adds a variety of useful aliases and functions for searching the web from the shell, including shortcuts for searching `Google`, `DuckDuckGo`, and `StackOverflow`.

```shell
google what's the meaning of life?
```

#### Auto suggestions

The [`zsh-autosuggestions`](https://github.com/zsh-users/zsh-autosuggestions) plugin adds auto-suggestions to the shell, making it easier to run commands by suggesting commands that have been previously run.

We'll need to clone the `zsh-autosuggestions` repository into the `~/.oh-my-zsh/plugins` directory:

```shell
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
```

#### Syntax highlighting

The [`zsh-syntax-highlighting`](https://github.com/zsh-users/zsh-syntax-highlighting.git) plugin adds syntax highlighting to the shell, making it easier to read commands and spot errors.

We'll need to clone the `zsh-syntax-highlighting` repository into the `~/.oh-my-zsh/plugins` directory:

```shell
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

## Return

[Return to the top-level README](./../../README.md)
