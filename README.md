# 📘 PCA Reading Assignment

> An educational resource for learning **Principal Component Analysis (PCA)** — a fundamental dimensionality reduction technique in machine learning and data science.

[![CI](https://github.com/mnoumanhanif/Reading-Assigment/actions/workflows/ci.yml/badge.svg)](https://github.com/mnoumanhanif/Reading-Assigment/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/demo-GitHub%20Pages-brightgreen)](https://mnoumanhanif.github.io/Reading-Assigment/)

---

## 📖 Description

This repository is a reading assignment for the **Advanced Big Data Analytics** course (24K-8001). It provides a comprehensive exploration of PCA through two complementary learning resources:

1. **Interactive PCA Guide** — A web-based tutorial with step-by-step explanations, interactive visualizations, and mathematical notation.
2. **Practical PCA Implementation** — A Jupyter Notebook demonstrating PCA in Python, comparing manual calculations with scikit-learn.

## ✨ Key Features

- **Interactive Learning** — Step-by-step PCA walkthrough with clickable buttons and dynamic charts
- **Mathematical Rigor** — Full LaTeX-rendered equations for standardization, covariance, eigendecomposition
- **Hands-On Code** — Complete Python implementation using NumPy and scikit-learn
- **Visual Explanations** — Scatter plots, bar charts, and data transformation visualizations
- **Self-Contained** — No build step required; open HTML files directly in any browser

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Languages** | Python, HTML, CSS, JavaScript |
| **Data Science** | NumPy, scikit-learn, Pandas |
| **Visualization** | Matplotlib, Seaborn, Chart.js |
| **Math Rendering** | MathJax |
| **Styling** | Tailwind CSS |
| **Notebooks** | Jupyter Notebook |

## 📂 Project Structure

```
Reading-Assigment/
├── src/                                    # Main content files
│   ├── pca-interactive-guide.html          # Interactive web-based PCA tutorial
│   └── pca-practical-implementation.html   # Jupyter Notebook export with Python code
├── docs/                                   # Developer documentation
│   ├── setup.md                            # Installation and setup guide
│   ├── architecture.md                     # Project architecture overview
│   └── development.md                      # Development workflow
├── .github/                                # GitHub configuration
│   ├── workflows/ci.yml                    # CI pipeline
│   ├── ISSUE_TEMPLATE/                     # Issue templates
│   └── pull_request_template.md            # PR template
├── README.md                               # This file
├── CONTRIBUTING.md                         # Contribution guidelines
├── LICENSE                                 # MIT License
├── CHANGELOG.md                            # Version history
├── requirements.txt                        # Python dependencies
├── .gitignore                              # Git ignore rules
└── .editorconfig                           # Editor configuration
```

## 🚀 Installation

### View Online

Visit the live site: **[https://mnoumanhanif.github.io/Reading-Assigment/](https://mnoumanhanif.github.io/Reading-Assigment/)**

### View Locally

```bash
# Clone the repository
git clone https://github.com/mnoumanhanif/Reading-Assigment.git
cd Reading-Assigment

# Open the interactive guide in your browser
open src/pca-interactive-guide.html        # macOS
xdg-open src/pca-interactive-guide.html    # Linux
start src/pca-interactive-guide.html       # Windows
```

## 📋 Usage

### Learning Path

1. **Start with theory** — Open `src/pca-interactive-guide.html` to understand PCA concepts, the mathematical process, and real-world applications.
2. **Move to practice** — Open `src/pca-practical-implementation.html` to see PCA implemented in Python with NumPy and scikit-learn.
3. **Experiment** — Set up the Python environment and try modifying the code yourself.

### Python Environment (Optional)

To run or modify the Jupyter notebook:

```bash
python -m venv venv
source venv/bin/activate    # macOS/Linux
pip install -r requirements.txt
jupyter notebook
```

## 🧪 Testing

The CI pipeline validates:
- HTML file existence and structure
- Required documentation files
- Project directory structure

Run the checks locally:

```bash
# Verify HTML files exist
ls src/*.html

# Check HTML structure
for f in src/*.html; do grep -q "<html" "$f" && echo "✅ $f"; done
```

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:

- Reporting issues
- Submitting pull requests
- Content and code style standards

## 📚 Additional Resources

- [Principal Component Analysis — Wikipedia](https://en.wikipedia.org/wiki/Principal_component_analysis)
- [A Complete Guide to PCA in Machine Learning — Medium](https://medium.com/towards-data-science/a-complete-guide-to-principal-component-analysis-pca-in-machine-learning-664f34fc3e5a)
- [Step-By-Step Guide to PCA — Turing](https://www.turing.com/kb/guide-to-principal-component-analysis)

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 👤 Author

**mnoumanhanif** — [GitHub Profile](https://github.com/mnoumanhanif)

Course: Advanced Big Data Analytics (24K-8001)
