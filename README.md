# Replication Package

This repository contains all artifacts required to reproduce the results presented in the paper:

**"What Makes Time Series Forecasting Repositories Survive? A Decade-Long MSR Study of 45,003 GitHub Projects"**

The replication package includes:

- Data collection pipeline
- Repository processing pipeline
- Project classification procedures
- Final dataset generation
- Statistical analyses
- Reproduction of the paper's tables
- Reproduction of the paper's figures

## Available Artifacts

### GitHubDataCollection.ipynb

Notebook responsible for mining data from GitHub.

Main functionalities:

- Querying the GitHub REST API
- Metadata collection
- Repository filtering
- Raw dataset construction
- Exporting data to Parquet format
- 
## GitHub Token Configuration

To execute the data collection pipeline, define a GitHub Personal Access Token.

Example:

```python
import os

os.environ["GITHUB_TOKEN"] = "YOUR_TOKEN"
```
### GeraçãoGraficos.ipynb

Notebook responsible for reproducing the statistical results reported in the paper.

Main functionalities:

- Kruskal-Wallis tests
- Games-Howell post-hoc tests
- Kaplan-Meier Survival Analysis
- Cox Proportional Hazards Modeling
- Generation of Figures 1–4
- Generation of the paper's tables
