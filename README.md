# SQLGuard

What this is
------------
SQLGuard contains Jupyter notebooks with experiments and ablation studies for the "SQLGuard" project (notebooks analyze and run experiments on a bird-related dataset — file names reference BIRRD / full_dev). This repository is intended for reproducible data-science experiments run interactively (Google Colab or local Jupyter).

Notebooks (top-level)
---------------------
- Ablation_Tests_Exp_3.ipynb
  - Ablation study notebook for Experiment 3. Contains analysis cells and experiment runs.
- Ablation_Tests_For_Experiment_2.ipynb
  - Ablation study notebook for Experiment 2. Contains the inputs, evaluation and visualization for that experiment.
- SQLGuard_Full_DEV_BIRRD_With1st_Ablation.ipynb
  - Main/full development notebook that runs the SQLGuard pipeline on the BIRRD (bird) dataset and includes the first ablation tests.

Quick overview
--------------
- These notebooks were authored to run experiments interactively (the notebooks' metadata indicate use with Google Colab/Jupyter).
- They expect experiment data to be on a mounted Google Drive path in Colab (examples in the notebooks refer to `/content/drive/.../SQLGuard_BIRD/...` and similar). Update the DATA_DIR variable in each notebook to point to your dataset location.
- Notebooks may produce large outputs and visualizations; Colab (with sufficient RAM) is recommended for heavy runs.

Requirements
------------
- Python 3.8+ (or appropriate Python 3 kernel used by your Jupyter/Colab environment)
- Jupyter / Google Colab
- Typical data-science packages (install with pip). Example:
  - pandas, numpy, matplotlib, seaborn, scikit-learn, ipywidgets
- If you use Colab: no kernel install is necessary, but you must mount Google Drive and pip-install any missing packages at the top of a notebook cell.

Suggested minimal install (local)
```bash
python -m venv venv
source venv/bin/activate        # or venv\Scripts\activate on Windows
pip install --upgrade pip
pip install jupyter pandas numpy matplotlib seaborn scikit-learn ipywidgets
