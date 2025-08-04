# Development Guidelines

## Universal Tool Usage

Always prefer **uv** for ALL development tasks it can handle in this project.

uv is an extremely fast Python package manager and development tool written in Rust. It provides:
- Faster dependency resolution and installation
- Better compatibility with modern Python packaging standards
- Improved performance over traditional tools like pip, virtualenv, pyenv, etc.
- Comprehensive project management capabilities

## Package Management

Use uv commands instead of pip:
- `uv add <package>` instead of `pip install <package>`
- `uv remove <package>` instead of `pip uninstall <package>`
- `uv sync` to install dependencies from pyproject.toml
- `uv lock` to generate/update the lock file
- `uv tree` to display dependency tree
- `uv export` to export lockfile to alternate formats

## Virtual Environment Management

Use uv instead of virtualenv/venv:
- `uv venv` to create a virtual environment
- `uv venv --python 3.11` to create with specific Python version
- `uv venv .venv` to create in specific directory
- Virtual environments are automatically managed with `uv sync`

## Python Version Management

Use uv instead of pyenv/python-build:
- `uv python list` to list available Python versions
- `uv python install 3.11` to install Python 3.11
- `uv python install 3.12.0` to install specific version
- `uv python find` to find Python installations
- `uv python pin 3.11` to pin project to Python version

## Project Management

Use uv for project lifecycle:
- `uv init` to create a new project
- `uv init --lib` to create a library project
- `uv init --app` to create an application project
- `uv version` to read/update project version

## Running Code

Use uv to run scripts and tools:
- `uv run <script.py>` to run Python scripts
- `uv run --with <package> <script.py>` to run with additional dependencies
- `uv run python -m <module>` to run modules
- `uv tool run <tool>` to run tools without installing globally
- `uv tool install <tool>` to install tools globally

## Building and Publishing

Use uv for package distribution:
- `uv build` to build source distributions and wheels
- `uv publish` to upload distributions to PyPI
- `uv publish --repository <repo>` to publish to specific repository

## Cache Management

Use uv for cache operations:
- `uv cache clean` to clean the cache
- `uv cache dir` to show cache directory
- `uv cache prune` to remove unused cache entries

## General Principles

1. **Replace pip**: Use `uv add/remove/sync` instead of `pip install/uninstall`
2. **Replace virtualenv**: Use `uv venv` instead of `python -m venv` or `virtualenv`
3. **Replace pyenv**: Use `uv python` for Python version management
4. **Replace python directly**: Use `uv run python` for script execution
5. **Replace build tools**: Use `uv build` instead of `python -m build`
6. **Replace twine**: Use `uv publish` instead of `twine upload`

Always check `uv --help` or `uv <command> --help` for the latest options and capabilities.