# Project Template for Energy Utopia Challenge

This template provides a starting structure for your Energy Utopia Challenge project. Copy and adapt it for your chosen topic.

---

## 📁 Recommended Project Structure

```
energy-utopia-project/
│
├── README.md                           # Project documentation
├── requirements.txt                    # Python dependencies
├── .gitignore                         # Git ignore file
├── LICENSE                            # License (if applicable)
│
├── data/                              # Data directory
│   ├── raw/                          # Original, immutable data
│   ├── interim/                      # Intermediate data
│   ├── processed/                    # Final processed data
│   └── README.md                     # Data documentation
│
├── notebooks/                         # Jupyter notebooks
│   ├── 01_data_collection.ipynb     # Data gathering
│   ├── 02_exploratory_analysis.ipynb # EDA
│   ├── 03_preprocessing.ipynb       # Data cleaning
│   ├── 04_feature_engineering.ipynb # Feature creation
│   ├── 05_modeling.ipynb            # Model training
│   └── 06_evaluation.ipynb          # Results analysis
│
├── src/                               # Source code
│   ├── __init__.py
│   ├── config.py                     # Configuration
│   │
│   ├── data/                         # Data processing
│   │   ├── __init__.py
│   │   ├── collect.py               # Data collection
│   │   ├── preprocess.py            # Preprocessing
│   │   └── features.py              # Feature engineering
│   │
│   ├── models/                       # Model definitions
│   │   ├── __init__.py
│   │   ├── train.py                 # Training logic
│   │   ├── predict.py               # Inference logic
│   │   └── evaluate.py              # Evaluation metrics
│   │
│   └── utils/                        # Utilities
│       ├── __init__.py
│       └── helpers.py               # Helper functions
│
├── models/                            # Saved models
│   ├── checkpoints/                  # Training checkpoints
│   └── final/                        # Final trained models
│
├── results/                           # Results and outputs
│   ├── figures/                      # Plots and visualizations
│   ├── metrics/                      # Performance metrics
│   └── predictions/                  # Model predictions
│
├── deployment/                        # Deployment files
│   ├── app.py                        # Web application
│   ├── Dockerfile                    # Docker configuration
│   ├── requirements-deploy.txt       # Deployment dependencies
│   └── static/                       # Static files for web app
│
├── reports/                           # Project reports
│   ├── proposal.pdf                  # Phase 1 proposal
│   ├── final_report.pdf             # Phase 2 report
│   └── figures/                      # Report figures
│
├── presentation/                      # Presentation materials
│   ├── slides.pdf                    # Final presentation
│   └── demo_video.mp4               # Demo video
│
└── tests/                             # Unit tests (optional)
    ├── __init__.py
    ├── test_data.py
    └── test_models.py
```

---

## 📝 Template Files

### 1. README.md Template

```markdown
# [Your Project Name]

**Energy Utopia Challenge - [Your Chosen Topic]**

## Overview
Brief description of your project and chosen topic.

## Problem Statement
Describe the specific problem you're solving.

## Approach
Explain your methodology and AI techniques.

## Data Sources
List all data sources used.

## Installation

\`\`\`bash
pip install -r requirements.txt
\`\`\`

## Usage

### Data Collection
\`\`\`bash
python src/data/collect.py
\`\`\`

### Training
\`\`\`bash
python src/models/train.py
\`\`\`

### Prediction
\`\`\`bash
python src/models/predict.py
\`\`\`

## Results
Summary of key results and metrics.

## Team
- **Note:** This section intentionally left anonymous for challenge submission

## License
MIT License (or your choice)
```

### 2. requirements.txt Template

```txt
# Core libraries
numpy>=1.21.0
pandas>=1.3.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=0.24.0

# Deep Learning (choose based on your needs)
# torch>=1.10.0
# tensorflow>=2.7.0

# Time Series (if applicable)
# statsmodels>=0.13.0
# prophet>=1.0

# Data Collection
requests>=2.26.0
beautifulsoup4>=4.10.0

# Utilities
jupyter>=1.0.0
notebook>=6.4.0
python-dotenv>=0.19.0
tqdm>=4.62.0

# Deployment (if applicable)
# flask>=2.0.0
# streamlit>=1.2.0
# fastapi>=0.70.0
```

### 3. .gitignore Template

```gitignore
# Python
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
env/
venv/
ENV/
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
*.egg-info/
.installed.cfg
*.egg

# Jupyter Notebook
.ipynb_checkpoints
*.ipynb_checkpoints

# Data files (adjust based on your needs)
data/raw/*
data/interim/*
data/processed/*
!data/raw/.gitkeep
!data/interim/.gitkeep
!data/processed/.gitkeep

# Models (large files)
models/checkpoints/*
models/final/*.h5
models/final/*.pt
models/final/*.pkl
!models/checkpoints/.gitkeep
!models/final/.gitkeep

# IDE
.vscode/
.idea/
*.swp
*.swo
*~

# OS
.DS_Store
Thumbs.db

# Environment variables
.env
.env.local

# Logs
*.log
logs/

# Temporary files
tmp/
temp/
*.tmp
```

### 4. src/config.py Template

```python
"""
Configuration file for the project
"""
import os
from pathlib import Path

# Project paths
PROJECT_ROOT = Path(__file__).parent.parent
DATA_DIR = PROJECT_ROOT / "data"
RAW_DATA_DIR = DATA_DIR / "raw"
PROCESSED_DATA_DIR = DATA_DIR / "processed"
MODELS_DIR = PROJECT_ROOT / "models"
RESULTS_DIR = PROJECT_ROOT / "results"

# Create directories if they don't exist
for dir_path in [RAW_DATA_DIR, PROCESSED_DATA_DIR, MODELS_DIR, RESULTS_DIR]:
    dir_path.mkdir(parents=True, exist_ok=True)

# Data collection settings
DATA_SOURCES = {
    "source1": "https://api.example.com/data",
    "source2": "path/to/local/data"
}

# Model hyperparameters (adjust based on your model)
MODEL_PARAMS = {
    "learning_rate": 0.001,
    "batch_size": 32,
    "epochs": 100,
    "random_state": 42
}

# Evaluation metrics
METRICS = ["mae", "rmse", "r2"]  # Adjust based on your task

# Random seed for reproducibility
RANDOM_SEED = 42
```

### 5. src/data/collect.py Template

```python
"""
Data collection script
"""
import pandas as pd
from pathlib import Path
import sys
sys.path.append(str(Path(__file__).parent.parent.parent))

from src.config import RAW_DATA_DIR, DATA_SOURCES

def collect_data():
    """
    Collect data from various sources
    """
    print("Starting data collection...")
    
    # Example: Load from CSV
    # df = pd.read_csv(DATA_SOURCES["source1"])
    
    # Example: API call
    # response = requests.get(DATA_SOURCES["source2"])
    # data = response.json()
    
    # Example: Web scraping
    # soup = BeautifulSoup(response.content, 'html.parser')
    
    # Save raw data
    # df.to_csv(RAW_DATA_DIR / "raw_data.csv", index=False)
    
    print(f"Data saved to {RAW_DATA_DIR}")
    
if __name__ == "__main__":
    collect_data()
```

### 6. src/models/train.py Template

```python
"""
Model training script
"""
import pandas as pd
import numpy as np
from pathlib import Path
import sys
sys.path.append(str(Path(__file__).parent.parent.parent))

from src.config import PROCESSED_DATA_DIR, MODELS_DIR, MODEL_PARAMS, RANDOM_SEED

def train_model():
    """
    Train the AI model
    """
    print("Loading processed data...")
    # df = pd.read_csv(PROCESSED_DATA_DIR / "processed_data.csv")
    
    print("Preparing features and target...")
    # X = df.drop('target', axis=1)
    # y = df['target']
    
    print("Training model...")
    # model = YourModel(**MODEL_PARAMS)
    # model.fit(X, y)
    
    print("Saving model...")
    # joblib.dump(model, MODELS_DIR / "final" / "model.pkl")
    
    print("Training complete!")

if __name__ == "__main__":
    train_model()
```

---

## 🚀 Quick Start Guide

### 1. Set Up Your Environment

```bash
# Clone/create your repository
git clone <your-repo-url>
cd your-project

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Collect Data

```bash
# Run data collection script
python src/data/collect.py

# Or use Jupyter notebook
jupyter notebook notebooks/01_data_collection.ipynb
```

### 3. Explore and Preprocess

```bash
# Open exploratory analysis notebook
jupyter notebook notebooks/02_exploratory_analysis.ipynb
```

### 4. Train Your Model

```bash
# Run training script
python src/models/train.py
```

### 5. Evaluate

```bash
# Run evaluation
python src/models/evaluate.py
```

---

## 📊 Data Documentation Template

Create a `data/README.md` file:

```markdown
# Data Documentation

## Data Sources

### Source 1: [Name]
- **URL/Location:** [link or path]
- **Description:** [brief description]
- **Format:** CSV/JSON/API
- **Size:** [number of records]
- **Time Period:** [date range]
- **License:** [if applicable]

### Source 2: [Name]
[Same structure as above]

## Data Fields

| Field Name | Type | Description | Example |
|------------|------|-------------|---------|
| timestamp | datetime | Time of measurement | 2025-01-01 12:00:00 |
| value | float | Energy consumption (kWh) | 125.5 |
| ... | ... | ... | ... |

## Data Quality Issues

- Missing values: [describe]
- Outliers: [describe]
- Inconsistencies: [describe]

## Preprocessing Steps

1. [Step 1]
2. [Step 2]
3. [Step 3]
```

---

## 📈 Tips for Each Topic

### For Energy Consumption:
- Look for smart meter datasets
- Consider time-of-day patterns
- Include weather data
- Focus on anomaly detection

### For Energy Storage:
- Battery cycle data is key
- Track degradation over time
- Temperature is important
- Model state-of-charge (SOC)

### For Renewable Energy:
- Weather data is essential
- Solar irradiance, wind speed
- Historical production data
- Seasonal patterns matter

### For Predictive Maintenance:
- Sensor data (vibration, temp)
- Failure logs/history
- Operating conditions
- Use classification models

---

## 🔍 Evaluation Checklist

Before submitting, ensure:

- [ ] Code is well-documented
- [ ] Repository is anonymous
- [ ] README is comprehensive
- [ ] All notebooks run without errors
- [ ] Results are reproducible
- [ ] Requirements.txt is complete
- [ ] Data sources are documented
- [ ] Model is saved and loadable
- [ ] Evaluation metrics are clear
- [ ] Code follows best practices

---

## 📞 Need Help?

Refer to:
- Main README.md for detailed challenge information
- README.fr.md for French documentation
- QUICK_REFERENCE.md for key dates and checklist

Contact: pes@ieee.tn or yp@ieee.tn

---

**Good luck with your project!** 🚀
