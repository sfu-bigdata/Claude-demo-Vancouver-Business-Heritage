# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Vancouver Business Heritage Proximity Predictor - A machine learning project to predict whether a Vancouver business is located near a heritage site.

**Data Sources:**
- Business licenses from City of Vancouver Open Data Portal
- Heritage sites from Vancouver Heritage Register
- See [DATA_SOURCES.md](DATA_SOURCES.md) for detailed information

**Project Plan:** See [PROJECT_PLAN.md](PROJECT_PLAN.md) for 5-task implementation roadmap

## Development Setup

This is a Python project. Setup instructions:

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On macOS/Linux

# Install dependencies (once requirements.txt is created)
pip install -r requirements.txt
```

## Project Structure

```
.
├── data/
│   ├── raw/              # Raw downloaded datasets
│   └── processed/        # Processed datasets (to be created)
├── src/
│   ├── preprocessing/    # Data preprocessing scripts (to be created)
│   └── models/          # ML model training scripts (to be created)
├── notebooks/           # Jupyter notebooks for EDA (to be created)
├── models/             # Saved trained models (to be created)
├── reports/            # Analysis reports and figures (to be created)
├── DATA_SOURCES.md     # Documentation of data sources
├── PROJECT_PLAN.md     # 5-task project implementation plan
└── README.md           # Project overview and usage instructions
```

## Development Practices

### Documentation
- **Always update README.md and other relevant documentation files whenever you add or update code**
- Keep DATA_SOURCES.md updated if new data sources are added
- Document methodology and decisions in notebooks

### Version Control
- **Commit often and push code at every checkpoint**
- Use descriptive commit messages
- Commit after completing each significant task or milestone

### Code Quality
- Write clean, well-documented Python code
- Include docstrings for functions and classes
- Create unit tests for data processing and feature engineering functions
