# datafun-07-ml

[![Docs Deploy](https://github.com/gracetulsi/datafun-07-ml/actions/workflows/deploy-mkdocs.yml/badge.svg?branch=main)](https://github.com/gracetulsi/datafun-07-ml/actions/workflows/deploy-mkdocs.yml)
[![CI](https://github.com/gracetulsi/datafun-07-ml/actions/workflows/ci-basic-mkdocs.yml/badge.svg?branch=main)](https://github.com/gracetulsi/datafun-07-ml/actions/workflows/ci-basic-mkdocs.yml)
[![Docs](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://gracetulsi.github.io/datafun-07-ml/)
[![Python](https://img.shields.io/badge/python-3.14-blue?logo=python&logoColor=white)](https://www.python.org/)

> Professional Python project: time series analysis, simple linear regression, and predictive analytics with Jupyter notebooks.

## Overview

This project explores introductory machine learning concepts including time series data, simple linear regression, and predictive analytics using Python, Jupyter notebooks, pandas, and scikit-learn. The analysis is part of Module 7 for the Data Analytics Fundamentals course (44-608).

**Author:** [Grace Tulsi](https://github.com/gracetulsi)

**Date:** February 2026

## Dataset

*To be determined.*

## Initial Setup

Following the [pro-analytics-02](https://gracetulsi.github.io/pro-analytics-02/) workflow:

1. Copied the `datafun-04-notebooks` template repo on GitHub and named it `datafun-07-ml`.
2. Configured repository settings:
   - Settings > Pages > Build and deployment > Source: **GitHub Actions**
   - Settings > Advanced Security > Dependabot > **Dependabot security updates**: Enabled
   - Settings > Advanced Security > Dependabot > **Grouped security updates**: Enabled
3. Opened a machine terminal (PowerShell) in my `Repos` folder and cloned the repo:

```shell
git clone https://github.com/gracetulsi/datafun-07-ml
```

4. Changed into the project directory and opened it in VS Code:

```shell
cd datafun-07-ml
code .
```

5. Installed recommended VS Code extensions when prompted.
6. Opened a VS Code terminal and set up the project Python environment:

```shell
uv self update
uv python pin 3.14
uv sync --extra dev --extra docs --upgrade
```

7. Clicked **Yes** when prompted to select the new environment for the workspace folder.
8. Installed and ran pre-commit checks (optional recommended):

```shell
uvx pre-commit install
git add -A
uvx pre-commit run --all-files
git add -A
uvx pre-commit run --all-files
```

9. Selected the project `.venv` interpreter using the Command Palette (`Ctrl+Shift+P` > `Python: Select Interpreter` > chose the Workspace `.venv`).
10. Ran `Developer: Reload Window` from the Command Palette (`Ctrl+Shift+P`) to ensure VS Code fully recognized the new environment.

## Repeatable Workflow

```shell
git pull
uv sync --extra dev --extra docs --upgrade
```

Run notebooks, make changes, then:

```shell
git add .
git commit -m "Descriptive message"
git push -u origin main
```

## Resources

- [Pro-Analytics-02](https://gracetulsi.github.io/pro-analytics-02/) - guide to professional Python
