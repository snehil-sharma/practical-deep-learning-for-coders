# Lesson 1: Getting Started with Deep Learning

This directory contains notebooks for the first lesson of the Practical Deep Learning for Coders course.

## Notebooks

### jupyter-notebook-101.ipynb
A basic introduction to using Jupyter notebooks, covering:
- Cell types and execution
- Markdown formatting
- Python basics in notebooks
- Running shell commands

### is-it-a-bird-creating-a-model-from-your-own-data.ipynb
A practical tutorial that builds an image classifier to distinguish birds from forests, demonstrating:

- Using DuckDuckGo search to collect image data
- Data preparation with FastAI
- Fine-tuning a pre-trained ResNet18 model
- Evaluating model performance
- Making predictions on new images

This notebook recreates the bird classifier from the famous XKCD comic that joked about the difficulty of computer vision - showing how something that was considered extremely difficult just a few years ago is now achievable in minutes.

## Running These Notebooks

From the project root directory:

```bash
uv sync  # Install required dependencies
uv run jupyter lab  # Start Jupyter Lab
```

Then navigate to the desired notebook in the Jupyter interface.

## Required Dependencies

- fastai
- duckduckgo_search (>= 6.2)
- fastcore
- fastdownload
- Pillow
- matplotlib
