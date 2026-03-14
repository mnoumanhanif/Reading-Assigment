# Development Guide

This guide covers the development workflow for contributing to the PCA Reading Assignment project.

## Development Environment

### Required Tools

- **Web browser** (Chrome/Firefox recommended for DevTools)
- **Text editor** with HTML/CSS support (VS Code recommended)
- **Git** for version control

### Recommended VS Code Extensions

- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) — Local development server with hot reload
- [HTML CSS Support](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css) — HTML/CSS IntelliSense
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) — Code formatter
- [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) — Consistent coding styles

## Workflow

### 1. Set Up Your Environment

```bash
# Fork and clone the repository
git clone https://github.com/<your-username>/Reading-Assigment.git
cd Reading-Assigment

# Create a feature branch
git checkout -b feature/your-feature-name
```

### 2. Make Changes

Edit files in the `src/` directory:

- **`src/pca-interactive-guide.html`** — The interactive web tutorial
- **`src/pca-practical-implementation.html`** — The Jupyter notebook export

### 3. Preview Changes

Open the HTML files directly in your browser, or use a local server:

```bash
# Using Python's built-in server
python -m http.server 8000

# Then visit http://localhost:8000/src/pca-interactive-guide.html
```

Or with VS Code Live Server:
1. Right-click any HTML file in `src/`
2. Select "Open with Live Server"

### 4. Test Your Changes

Before committing, verify:

- [ ] HTML files open correctly in the browser
- [ ] All interactive elements work (buttons, tabs, charts)
- [ ] Mathematical equations render properly
- [ ] Content is accurate and well-formatted
- [ ] No broken links or missing resources

### 5. Commit and Push

```bash
git add .
git commit -m "Add: description of your change"
git push origin feature/your-feature-name
```

### 6. Open a Pull Request

Go to GitHub and open a pull request against the `main` branch.

## Content Guidelines

### Adding New Sections

When adding new content to the interactive guide:

1. Follow the existing section structure (header, content, examples).
2. Use Tailwind CSS classes for styling consistency.
3. Add interactive elements where they enhance understanding.
4. Include mathematical notation using MathJax syntax.

### Updating the Jupyter Notebook

If modifying the practical implementation:

1. Edit the original `.ipynb` file in Jupyter.
2. Run all cells to ensure correctness.
3. Export to HTML: `File > Download as > HTML (.html)`.
4. Replace `src/pca-practical-implementation.html` with the new export.

### Writing Documentation

- Use clear, accessible language.
- Include code examples where helpful.
- Follow Markdown best practices.
- Keep documentation in sync with the codebase.

## CI Pipeline

The GitHub Actions CI workflow (`.github/workflows/ci.yml`) runs on every push and pull request to `main`. It checks:

1. HTML files exist in `src/`
2. HTML structure is valid
3. Required documentation files are present
4. Project directory structure is correct

Check CI results on your pull request before requesting review.
