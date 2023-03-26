# iTerm2 - Terminal

`iTerm2` is a terminal emulator application for macOS that provides a more powerful and customizable alternative to the default macOS `Terminal`.
It is an open-source application that offers a variety of features for working with command-line interfaces, such as split panes, search, autocomplete and more.

## Installation

```shell
brew install --cask iterm2
```

Close the `terminal` application and open `iTerm` instead.
Any time I refer to the terminal in these guides, I mean the iTerm2 application.

## Setup

With the iTerm2 application open, go to `Preferences` and select the `Appearance` tab.
Within the `General` tab, set `Theme` to `Minimal`, and `Status Bar` to `Bottom`.

![iTerm2 Before](./images/iTerm2_pre.png)

In the `Profiles` tab, select the `Session` tab, and then check `Status bar enabled` at the bottom of the window and then click the `Configure Status Bar` button.

![iTerm2 Status Bar](./images/iTerm2_status_bar.png)

I like to have the `Battery Level`, `CPU Utilization`, `Memory Utilization`, `Network Throughput` in my status bar.

![iTerm2 After](./images/iTerm2_post.png)

## Neofetch

As a bonus, I like to have a little bit of information about my system displayed in the terminal when I open it.
We can use the `neofetch` command to display this information.
We'll install it using Homebrew:

```shell
brew install neofetch
```

Then, we'll add the following line to our `~/.zprofile` file:

```shell
echo "neofetch" >> ~/.zprofile
```

Next time we open the terminal, we'll see the following information displayed:

![Neofetch](./images/Neofetch.png)

My terminal is slightly transparent, so you can see the desktop wallpaper behind it.
Yours will probably be a more sensible solid black!

## Return

[Return to the top-level README](./../../README.md)
