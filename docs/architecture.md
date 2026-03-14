# Project Architecture

This document describes the architecture and structure of the PCA Reading Assignment project.

## Overview

The project is an educational resource for learning **Principal Component Analysis (PCA)**, a fundamental dimensionality reduction technique in machine learning and data science. It consists of two main components: an interactive web-based guide and a practical Python implementation.

## Project Structure

```
Reading-Assigment/
├── src/                                    # Main content files
│   ├── pca-interactive-guide.html          # Interactive web-based PCA tutorial
│   └── pca-practical-implementation.html   # Jupyter Notebook export with Python code
├── docs/                                   # Developer documentation
│   ├── setup.md                            # Installation and setup guide
│   ├── architecture.md                     # This file
│   └── development.md                      # Development workflow
├── .github/                                # GitHub configuration
│   ├── workflows/
│   │   └── ci.yml                          # CI pipeline
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md                   # Bug report template
│   │   └── feature_request.md              # Feature request template
│   └── pull_request_template.md            # PR template
├── README.md                               # Project overview
├── CONTRIBUTING.md                         # Contribution guidelines
├── LICENSE                                 # MIT License
├── CHANGELOG.md                            # Version history
├── requirements.txt                        # Python dependencies
├── .gitignore                              # Git ignore rules
└── .editorconfig                           # Editor configuration
```

## Content Components

### 1. Interactive PCA Guide (`src/pca-interactive-guide.html`)

A self-contained, interactive web tutorial that teaches PCA concepts step by step.

**Technology Stack:**
- **Tailwind CSS** — Responsive styling via CDN
- **Chart.js** — Interactive data visualizations (scatter plots, bar charts)
- **MathJax** — LaTeX mathematical equation rendering
- **Vanilla JavaScript** — Interactive UI logic

**Key Sections:**
1. Overview of dimensionality reduction
2. Step-by-step PCA process (interactive walkthrough)
3. Numerical example with sample data
4. Visualizations of data before and after PCA
5. Pros and cons analysis
6. Real-world applications

**Interactive Features:**
- Tab-based navigation
- Step-by-step data transformation buttons
- Dynamic chart rendering
- Mathematical formula display

### 2. Practical PCA Implementation (`src/pca-practical-implementation.html`)

A Jupyter Notebook exported to HTML, demonstrating PCA implementation in Python.

**Technology Stack:**
- **Python** with NumPy, scikit-learn, Matplotlib, Seaborn
- **Jupyter Notebook** styling and layout

**Key Topics:**
1. Manual PCA calculation using NumPy:
   - Data standardization
   - Covariance matrix computation
   - Eigendecomposition
   - Data projection onto principal components
2. Scikit-learn PCA implementation
3. Comparison and validation between manual and library approaches
4. Data visualizations

## External Dependencies

All external dependencies are loaded via CDN (no build step required):

| Library | Version | Purpose |
|---------|---------|---------|
| Tailwind CSS | 3.x | Styling |
| Chart.js | 4.x | Data visualization |
| MathJax | 3.x | Math rendering |
| Polyfill.io | Latest | Browser compatibility |

## Deployment

The project is deployed as a static site via **GitHub Pages**, serving HTML files directly without any build process.

**Live URL:** [https://mnoumanhanif.github.io/Reading-Assigment/](https://mnoumanhanif.github.io/Reading-Assigment/)
