# Setup Guide

This guide walks you through setting up the PCA Reading Assignment project on your local machine.

## Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Git installed on your machine
- Python 3.8+ (optional, for running the Jupyter notebook)

## Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/mnoumanhanif/Reading-Assigment.git
cd Reading-Assigment
```

### 2. View the Content

Open the HTML files directly in your browser:

```bash
# Interactive PCA Guide
open src/pca-interactive-guide.html     # macOS
xdg-open src/pca-interactive-guide.html # Linux
start src/pca-interactive-guide.html    # Windows

# Practical PCA Implementation
open src/pca-practical-implementation.html     # macOS
xdg-open src/pca-practical-implementation.html # Linux
start src/pca-practical-implementation.html    # Windows
```

### 3. Online Access

The content is also available online via GitHub Pages:

🔗 [https://mnoumanhanif.github.io/Reading-Assigment/](https://mnoumanhanif.github.io/Reading-Assigment/)

## Python Environment Setup (Optional)

If you want to run or modify the Jupyter notebook that generated the practical implementation:

### 1. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

## Troubleshooting

| Issue | Solution |
|-------|----------|
| HTML file doesn't load | Ensure you're opening the file directly in a browser, not a text editor |
| Mathematical equations not rendering | Check your internet connection (MathJax loads from CDN) |
| Charts not displaying | Ensure JavaScript is enabled in your browser |
| Python dependencies fail to install | Try upgrading pip: `pip install --upgrade pip` |
