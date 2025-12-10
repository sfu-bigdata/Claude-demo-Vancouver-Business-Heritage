# Vancouver Business Heritage Proximity Predictor

A machine learning project that predicts whether a Vancouver business is located near a heritage site using data from the City of Vancouver Open Data Portal.

## Project Overview

This project analyzes the relationship between Vancouver businesses and heritage sites to predict proximity using geographic data and machine learning techniques. The model can help identify businesses near heritage locations, which may be useful for urban planning, tourism, and heritage conservation efforts.

## Current Status

**Task 1: Data Collection and Acquisition** ✅ COMPLETED
- Downloaded Vancouver business license dataset (132,635 businesses)
- Downloaded heritage sites dataset (2,495 heritage sites)
- Created comprehensive data documentation

**Next Steps:** Task 2 - Data Preprocessing and Feature Engineering

See [PROJECT_PLAN.md](PROJECT_PLAN.md) for full implementation roadmap.

## Data Sources

All datasets are from the City of Vancouver Open Data Portal under the Open Government Licence - Vancouver:

- **Business Licenses:** 132,635 active businesses with coordinates
- **Heritage Sites:** 2,495 heritage buildings, streetscapes, and landscape resources

For detailed information, see [DATA_SOURCES.md](DATA_SOURCES.md).

## Project Structure

```
.
├── data/
│   ├── raw/              # Raw downloaded datasets
│   │   ├── business_licences.csv
│   │   └── heritage_sites.csv
│   └── processed/        # Processed datasets (to be created)
├── src/
│   ├── preprocessing/    # Data preprocessing scripts (to be created)
│   └── models/          # ML model training scripts (to be created)
├── notebooks/           # Jupyter notebooks for EDA (to be created)
├── models/             # Saved trained models (to be created)
├── reports/            # Analysis reports and figures (to be created)
├── DATA_SOURCES.md     # Documentation of data sources
└── PROJECT_PLAN.md     # 5-task project implementation plan
```

## Setup

```bash
# Clone the repository
git clone https://github.com/sfu-bigdata/Claude-demo-Vancouver-Business-Heritage.git
cd Claude-demo-Vancouver-Business-Heritage

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On macOS/Linux
# or: venv\Scripts\activate  # On Windows

# Install dependencies (once requirements.txt is created)
pip install -r requirements.txt
```

## Usage

Data collection is complete. Implementation of preprocessing and modeling scripts is in progress.

## GitHub Issues

Track progress on [GitHub Issues](https://github.com/sfu-bigdata/Claude-demo-Vancouver-Business-Heritage/issues):
- Issue #2: Task 1 - Data Collection and Acquisition
- Issue #3: Task 2 - Data Preprocessing and Feature Engineering
- Issue #4: Task 3 - Exploratory Data Analysis
- Issue #5: Task 4 - Model Development and Training
- Issue #6: Task 5 - Model Evaluation and Documentation

## License

Data: Open Government Licence - Vancouver
Project Code: [To be determined]

## Attribution

Contains information licensed under the Open Government Licence – Vancouver.
