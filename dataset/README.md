# dataset

This folder contains dataset files used by the notebooks in this repository.

Files:
- `MNIST.mat` — MATLAB-format MNIST subset (used for image examples).
- `data.csv` — large CSV (≈73 MB) used as the main dataset for experiments.
- `train.csv` — training split CSV.
- `poly_regression_small.csv` — small polynomial regression dataset.
- `poly_regression_large.csv` — larger polynomial regression dataset for scalability tests.

Notes:
- `data.csv` exceeds GitHub's recommended file-size limits; consider using Git LFS for large binaries.
- Keep sensitive data out of the repository. Add a `.gitignore` entry if needed.
