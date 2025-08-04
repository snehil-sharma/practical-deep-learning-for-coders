# Development Guidelines

## Package Management

Always prefer **uv** for package management in this project.

uv is a fast Python package installer and resolver, written in Rust. It provides:
- Faster dependency resolution and installation
- Better compatibility with modern Python packaging standards
- Improved performance over traditional tools like pip

When working on this project, use uv commands instead of pip:
- `uv add <package>` instead of `pip install <package>`
- `uv remove <package>` instead of `pip uninstall <package>`
- `uv sync` to install dependencies from pyproject.toml
- `uv lock` to generate/update the lock file