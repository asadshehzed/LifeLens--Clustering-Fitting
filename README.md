## LifeLens: Clustering & Fitting

A compact, reproducible analysis of global life expectancy using clustering and curve fitting. Built around a single notebook for transparency and ease of exploration.

---

### Table of Contents
- About the Project
- Features
- Getting Started
- Configuration
- Roadmap
- Contributing
- License
- Acknowledgements

---

### About the Project
This project explores patterns in life expectancy across countries using unsupervised learning and simple statistical modeling. The goal is to provide an approachable, well-documented workflow that demonstrates:
- how to prepare and profile a real-world dataset,
- how clustering can reveal regional or socioeconomic groupings, and
- how curve fitting can capture basic relationships between health and development metrics.

The analysis lives in a single Jupyter notebook so readers can follow the narrative, rerun steps, and modify experiments without digging through a large codebase.

---

### Features
- Clean, end-to-end notebook: data loading → exploration → preprocessing → modeling → evaluation → visualization.
- K-means clustering with guidance on choosing the number of clusters (elbow/silhouette).
- Curve fitting and regression baselines for key relationships (e.g., life expectancy vs. GDP or health indicators).
- Clear visualizations: scatter plots, cluster overlays, and residual diagnostics.
- Reproducible setup with minimal dependencies.

---

### Getting Started

#### Prerequisites
- Python 3.9+ recommended
- pip

#### Install
```bash
# Clone the repository
git clone <your-fork-or-repo-url>
cd Clusting---Fitting-Assignment--Applied-Data-Science-1-main

# (Optional) create a virtual environment
python -m venv .venv
# Windows PowerShell
.\.venv\Scripts\Activate.ps1

# Install minimal dependencies
python -m pip install --upgrade pip
pip install jupyter pandas numpy scikit-learn matplotlib seaborn scipy
```

#### Run the notebook
```bash
jupyter notebook "Clustering and Fitting.ipynb"
```
Then run cells top-to-bottom.

If you prefer VS Code or another IDE, open the folder and run the notebook there.

---

### Configuration
By default, the notebook expects the dataset file to be present at the project root:
- `Life-Expectancy-Data-Averaged.csv`

Optional environment variable to override the dataset path:
```bash
# Example (PowerShell)
$env:LIFE_DATA_PATH = "C:\\path\\to\\Life-Expectancy-Data-Averaged.csv"
```
Update the corresponding data-loading cell in the notebook to read from `LIFE_DATA_PATH` if set.

---

### Roadmap
- Add alternative clustering algorithms (DBSCAN, Gaussian Mixture Models) and compare stability.
- Introduce feature scaling/selection variants and sensitivity analysis.
- Expand curve fitting with regularized models and non-linear baselines.
- Add interactive plots for exploring clusters and model residuals.
- Publish a lightweight `requirements.txt` and `environment.yml` for exact reproducibility.

---

### Contributing
Contributions are welcome. A good way to help:
- Open an issue describing a bug, gap, or enhancement.
- For small fixes, submit a focused pull request with a clear description and before/after notes.
- For larger changes, start a discussion first so we can agree on scope and approach.

Please keep code readable and the notebook narrative clear. Prefer incremental edits with short, descriptive commit messages.

---

### License
This project is licensed under the MIT License. See `LICENSE` if present, or open an issue if you need clarification.

---

### Acknowledgements
- Dataset: Life Expectancy Averaged by Shreyas G on Kaggle — see the data page for details and usage terms: [Kaggle: Life Expectancy Averaged Dataset](https://www.kaggle.com/datasets/shreyasg23/life-expectancy-averaged-dataset/data)
- Libraries: pandas, NumPy, scikit-learn, Matplotlib, Seaborn, SciPy.
- Inspiration: common data science workflows for unsupervised learning and model diagnostics.
