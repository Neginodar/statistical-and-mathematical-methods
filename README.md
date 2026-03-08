# Statistical and Math Notebooks

This folder contains four educational Jupyter notebooks that demonstrate key numerical, linear-algebra, optimization, and statistical techniques often used in machine learning and data analysis. Each notebook is self-contained with explanatory text, equations, plots, and runnable code cells so you can reproduce the results and adapt the examples.

Repository contents
- [01-condition-numbers-and-matrices.ipynb](01-condition-numbers-and-matrices.ipynb)
- [02-svd-pca-image-compression.ipynb](02-svd-pca-image-compression.ipynb)
- [03-gradient-descent-and-sgd.ipynb](03-gradient-descent-and-sgd.ipynb)
- [04-mle-map-polynomial-regression.ipynb](04-mle-map-polynomial-regression.ipynb)

What you'll learn
- Numerical stability and condition numbers: how small input changes can produce large output changes and how to measure that sensitivity.
- Matrix decompositions (SVD) and PCA: dimensionality reduction and practical image-compression using low-rank approximations.
- Optimization basics: batch Gradient Descent vs Stochastic Gradient Descent (SGD), learning rate effects, and convergence behavior.
- Statistical estimation: Maximum Likelihood Estimation (MLE) and Maximum A Posteriori (MAP) for polynomial regression and model selection.

Prerequisites
- Python 3.8 or newer.
- Basic familiarity with linear algebra (matrices, vectors), calculus (gradients), and probability/statistics.

Setup (recommended)

1. Create and activate a virtual environment (macOS / Linux):

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
```

2. Install dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

Quick usage

- Start Jupyter (Notebook or Lab) from this folder and open any notebook:

```bash
jupyter notebook
# or
jupyter lab
```

- In each notebook: set the kernel to the Python environment you installed the dependencies into, then use `Run -> Run All Cells` to reproduce plots and outputs.

Detailed per-notebook summary

- `01-condition-numbers-and-matrices.ipynb`
   - Topics: matrix norms, eigenvalues, condition numbers, effects of perturbations.
   - Exercises: compute condition numbers for sample matrices; visual demonstrations of instability.
   - Runtime: seconds for small matrices.

- `02-svd-pca-image-compression.ipynb`
   - Topics: SVD properties, PCA for dimensionality reduction, compressing images by truncating singular values.
   - Exercises: compress sample images at different ranks and compare reconstruction error and PSNR.
   - Data: uses small example images; ensure `pillow` is installed for image I/O.

- `03-gradient-descent-and-sgd.ipynb`
   - Topics: gradient descent algorithm, stochastic updates (SGD), learning rate schedules, batch size effects.
   - Exercises: tune hyperparameters to observe convergence and plot loss curves.
   - Notes: long runs (large datasets) can be slowed; sample sizes are small for demonstration.

- `04-mle-map-polynomial-regression.ipynb`
   - Topics: linear regression, polynomial basis expansion, MLE vs MAP, regularization, model evidence.
   - Exercises: compare polynomial degrees, visualize overfitting/underfitting, compute posterior distributions.

Reproducibility tips
- Restart the kernel and `Run All` to ensure a clean execution order.
- If outputs differ due to random seeds, set a fixed seed (e.g., `numpy.random.seed(0)`) at the top of each notebook.

Troubleshooting
- Kernel not finding packages: make sure the notebook kernel uses the same Python environment where you installed dependencies.
- Slow plots or large images: reduce sample sizes or image resolution in the notebook cells before running.

Files added/modified
- `requirements.txt` — minimal Python packages needed to run the notebooks.

Contributing
- These notebooks are meant for learning. If you'd like additional examples, clearer explanations, or tests, open an issue or suggest changes.

License & contact
- These materials are provided for educational use. Contact me if you want a different license or to request clarifications.

If you'd like, I can also automatically generate a `requirements.txt`, add example data, or create short HTML exports of each notebook.
