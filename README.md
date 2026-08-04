# BIG_DATA_CourseWork

This repository contains coursework artifacts for a big data pipeline and analytics workflow, organized by project phases and implemented primarily in Jupyter notebooks.

## Repository Structure

- `notebooks/` — Main project notebooks covering ingestion, cleaning, EDA, modeling, and visualization.
- `data/` — Input and intermediate datasets used by the notebooks.
- `db/` — SQLite/database artifacts generated during analysis workflows.
- `outputs/` — Produced outputs such as processed files, metrics, and plots.

## Notebooks Directory Contents

The `notebooks/` directory currently includes:

1. `Phase1And2.ipynb`
   - **Phase 1: Ingestion**
   - **Phase 1b: Fares**
   - **Phase 1c: Data Cleaning**
   - **Phase 1d: Data Augmentation**
   - **Phase 1e: Save to Parquet**
   - **Phase 2: EDA, Reliability Metrics & SQLite Storage**

2. `Phase3And4.ipynb`
   - **Phase 3**
   - **Phase 4**
   - Includes visual analysis sections, for example:
     - Model Performance Comparison
     - Actual vs Predicted Scatter
     - Average Delay by Hour
     - Delay Distribution KDE

## Prerequisites

- Python 3.9+ (recommended)
- Jupyter Notebook or JupyterLab

Suggested Python packages (install as needed based on notebook imports):

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `pyarrow`
- `sqlite3` (standard library)

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd BIG_DATA_CourseWork
   ```

2. (Optional but recommended) Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\\Scripts\\activate
   ```

3. Install dependencies:
   ```bash
   pip install jupyter pandas numpy matplotlib seaborn scikit-learn pyarrow
   ```

## How to Run the Notebooks

1. Start Jupyter:
   ```bash
   jupyter notebook
   ```
   or
   ```bash
   jupyter lab
   ```

2. Open notebooks in order for the intended workflow:
   - First: `notebooks/Phase1And2.ipynb`
   - Then: `notebooks/Phase3And4.ipynb`

3. Run cells sequentially from top to bottom in each notebook.

## Outputs and Data Artifacts

- Processed datasets and result files are expected in `outputs/`.
- Database artifacts used for storage/query steps are expected in `db/`.
- Input datasets should be kept in `data/` unless notebook paths specify otherwise.

## Notes

- If a cell fails due to missing files, confirm dataset locations under `data/`.
- If package-related errors occur, install missing dependencies and rerun the notebook kernel.
