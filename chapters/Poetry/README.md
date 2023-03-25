# Poetry - Virtual Environments Manager

Poetry is a tool for managing Python dependencies and packaging Python applications.
It provides an easy-to-use command-line interface for creating, publishing, and managing Python packages and their dependencies.

## Installation

You can install Poetry using Homebrew:

```shell
brew install poetry
```

## Usage

To create a new Python project, run the `poetry new` command with the name of the project:

```shell
poetry new my_project
```

You can then install the project's dependencies, and the `my_project` package itself using `poetry install`:

```shell
poetry install
```

You can then run a script (which may `import my_project`) using the following command:

```shell
poetry run python path/to/my_script.py
```

If you want to add a new dependency to the project, you can do so using the following command:

```shell
poetry add some_dependency
```

If you want to add a new development dependency to the project, you can do so using the following command:

```shell
poetry add --dev some_dev_dependency
```

To publish the project to `PyPI`, run the following command:

```shell
poetry publish
```

## Return

[Return to the top-level README](./../../README.md)
