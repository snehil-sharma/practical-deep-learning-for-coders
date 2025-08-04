# practical-deep-learning-for-coders
Fast AI Course Learning

## Setup

This project uses [uv](https://github.com/astral-sh/uv) for fast and reliable Python package management.

### Installation

1. Install uv if you haven't already:
   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. Install project dependencies:
   ```bash
   uv sync
   ```

### Development

- Add new dependencies: `uv add <package>`
- Remove dependencies: `uv remove <package>`
- Update lock file: `uv lock`
- Run Python scripts: `uv run <script.py>`
