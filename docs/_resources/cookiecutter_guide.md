---
title: CookieCutter Guide
layout: page
permalink: /cookiecutter-guide/
---

# CookieCutter

A cookiecutter template for those interested in developing computational molecular packages in Python. Skeletal starting repositories can be created from this template to create the file structure semi-autonomously, so you can focus on what's important: **the science!**

The skeletal structure is designed to help you get started, but do not feel limited by the skeleton's features included here. You can alter continuous integration options, remove deployment platforms, or test with a different suite.

---

## Advantages

### 1. Faster Project Setup

**Without Cookiecutter:**

- Manually create folders (`docs/`, `tests/`, `devtools/`)
- Manually write `pyproject.toml`, `setup.cfg`, `LICENSE`, etc.
- Manually initialize Git, set up CI/CD, and install dependencies

**With Cookiecutter:**

- A single command sets up everything:
  ```bash
  cookiecutter gh:molssi/cookiecutter-cms
  ```
- No need to manually copy-paste files across multiple projects

---

### 2. Standardized Structure Across Projects

- Consistent folder structure across team projects
- CI/CD, testing, and packaging set up the same way
- No confusion about where to place files

---

### 3. Built-in Best Practices

MolSSI’s Cookiecutter includes:

- Pre-configured GitHub Actions for CI/CD
- `pyproject.toml` for modern Python builds
- Automatic setup of testing (`pytest`)
- Option to include ReadTheDocs for documentation

---

### 4. Automation and Customization

Cookiecutter helps automate:

- Filling in all details like name, license, etc.
- Creating a predefined README
- Setting up pytest and Git hooks in seconds

---

## Step-by-step Guide

### Prerequisites

- Python 3.x installed
- Git installed
- VS Code or PyCharm (optional)
- macOS, Windows, or Linux terminal access
- GitHub account

---

### 1. Installing Cookiecutter

```bash
python3 -m pip install --upgrade pip
python3 -m pip install cookiecutter
```

#### Troubleshooting:
- ❗ If pip command not found → use `python3 -m pip`
- ❗ If installed but not found → add `~/Library/Python/3.x/bin` to PATH (Mac)

---

### 2. Creating a Project from a Template

```bash
cookiecutter gh:molssi/cookiecutter-cms
```

**Follow the prompts:**
- Project name
- License
- Dependency source (pip-only or conda-forge)
- Include ReadTheDocs? (usually "n")

#### Troubleshooting:
- ❗ Developer tools error → `xcode-select --install`
- ❗ Git clone fails → check with `git --version`

---

### 3. Navigating the Created Project

Your repo will contain:

| File/Folder          | Purpose                                             |
|----------------------|-----------------------------------------------------|
| `README.md`          | Main documentation                                  |
| `LICENSE`            | Selected open-source license                        |
| `CODE_OF_CONDUCT.md` | Community guidelines                                |
| `pyproject.toml`     | Modern Python build config                          |
| `setup.cfg`          | Project metadata and dependencies                   |
| `MANIFEST.in`        | Extra packaging files                               |
| `devtools/`          | CI/CD configurations                                |
| `docs/`              | Documentation setup                                 |
| `samplerepo/`        | Main Python package                                 |

---

## Start Coding

Create your Python file inside `samplerepo/`, and add code and tests.

---

## Run Pytest

```bash
python3 -m pip install pytest
python3 -m pytest
```

Ensure pytest is in your PATH:

```bash
which pytest
```

If not:

```bash
export PATH="$HOME/Library/Python/3.13/bin:$PATH"
```

Make it permanent:

```bash
echo 'export PATH="$HOME/Library/Python/3.13/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

---

## Git Troubleshooting

If you get this error:

```
git commit -m "Initial commit after CMS Cookiecutter creation..." returned non-zero exit status 128.
```

It likely means Git isn't configured. Fix it:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

## Git Workflow After Pytest

1. Stage your changes:
```bash
git add .
```

2. Confirm changes:
```bash
git status
```

3. Commit:
```bash
git commit -m "Added Fibonacci function and tests after running pytest"
```

4. Push:
```bash
git push -u origin main
```

#### ⚠️ Git 403 Error?

Use a Personal Access Token (PAT) instead of your password.  
See: [GitHub Access Token Setup](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
