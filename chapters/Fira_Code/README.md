# Fira Code - Font

The Fira Code font is a monospaced font that includes programming ligatures, making it easier to read and write code.

## Installation

You can install Fira Code using Homebrew:

```shell
brew tap homebrew/cask-fonts
brew install --cask font-fira-code
```

To use the font in iTerm2 open the `Preferences` menu and navigate to the `Profiles` tab, and then select the `Text` tab.
Select the `Fira Code` font, then check `Use ligatures`.

To enable ligatures in VSCode, open `Settings` and add the following to the `settings.json` file:

```json
"editor.fontFamily": "Fira Code",
"editor.fontLigatures": true
```

## Return

[Return to the top-level README](./../../README.md)
