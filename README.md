# Practical Deep Learning for Coders

This project is set up for experimenting with and running notebooks from the [fast.ai Practical Deep Learning for Coders](https://course.fast.ai/) course.

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

### Dependencies

The project includes all necessary dependencies for the fast.ai course:
- **Jupyter Lab/Notebook** - For running interactive notebooks
- **fastai** - The main fast.ai library with PyTorch backend
- **matplotlib** - For plotting and visualization
- **pandas, numpy, scikit-learn** - Core data science libraries
- **torch, torchvision** - PyTorch deep learning framework

## Running Notebooks

### Start Jupyter Lab
```bash
uv run jupyter lab
```

This will start Jupyter Lab and open it in your browser. Navigate to the `notebooks/` directory to access course notebooks.

### Start Jupyter Notebook (alternative)
```bash
uv run jupyter notebook
```

## Project Structure

```
practical-deep-learning-for-coders/
├── notebooks/           # Course notebooks organized by lesson
│   ├── self/           # Personal exploratory notebooks
│   │   └── fastai-intro.ipynb
│   ├── kaggle/         # Notebooks from Kaggle sources
│   │   └── lesson01/   # Lesson 1: Jupyter Notebook basics
│   │       └── jupyter-notebook-101.ipynb
│   └── README.md       # Notebooks organization guide
├── pyproject.toml      # Project configuration and dependencies
├── uv.lock            # Locked dependency versions
└── README.md          # This file
```

## Adding New Lessons

When you download new notebooks from the course:

1. Create a new lesson directory:
   ```bash
   mkdir notebooks/lessonXX
   ```

2. Download the notebook from Kaggle and place it in the lesson directory

3. Update the notebooks README.md with the new lesson information

## Development

- Add new dependencies: `uv add <package>`
- Remove dependencies: `uv remove <package>`
- Update lock file: `uv lock`
- Run Python scripts: `uv run <script.py>`

## Course Resources

- [Course Website](https://course.fast.ai/)
- [Course Book](https://github.com/fastai/fastbook)
- [fast.ai Documentation](https://docs.fast.ai/)
