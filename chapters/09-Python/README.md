# Python - Language Interpreter

Python is a programming language that is used to write high-level code.

## Installation

Although a version of the Python interpreter is already installed on your computer, you can install a newer version using Homebrew:

```shell
brew install python
```

By default, the interpreter will be installed under the command `python3`.
If you'd like to call it with just `python` you can create an alias for the command and add it to your shell's start-up script:

```shell
echo 'alias python="python3"' >> ~/.zprofile
```

## Usage

If you were to use Python as is it will write everything into the global workspace, which is not ideal.

Instead, you should use Poetry (explained in the next chapter) to create a new project and install/manage the dependencies you need.

If you REALLY to use Python without Poetry, you can create a new virtual environment using the following command:

```shell
python -m venv my_project_venv
```

You can then activate the project using the following command:

```shell
source my_project_venv/bin/activate
```

You can then install a dependency using the following command:

```shell
pip install some_dependency
```

You can then run a script using the following command:

```shell
python path/to/my_script.py
```

## Return

[Return to the top-level README](./../../README.md)
