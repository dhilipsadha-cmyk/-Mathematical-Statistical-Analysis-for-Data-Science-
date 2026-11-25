# Mathematical & Statistical Analysis for Data Science

Module 3 – Assignment 1 (Mathematics and Statistics for Data Science)

This project analyses business data using **Linear Algebra**, **Probability** and **Descriptive Statistics** in Python, with NumPy, Pandas, SciPy and Matplotlib.

## Project structure

```
math-stats-assignment/
├── Mathematics_for_Data_Science_Assignment.ipynb   # main notebook (all 3 tasks)
├── requirements.txt                                # packages for the virtual environment
├── README.md
└── .gitignore                                      # keeps .venv out of git
```

## What the notebook covers

| Task | Topics |
|------|--------|
| 1. Linear Algebra | Vector addition, subtraction, dot product; matrix addition and multiplication; determinant, inverse, eigenvalues and eigenvectors of `matrix_a` |
| 2. Probability | Probability of successful sales; conditional probability by customer segment; Bayes' theorem; binomial simulation (20 trials); normal and uniform distributions |
| 3. Descriptive Statistics | Mean, median, mode; range, variance, standard deviation; skewness and kurtosis; interpretation of symmetry |

## Key results

- **Dot product** of `vector_a` and `vector_b`: 44
- **Determinant** of `matrix_a`: 6, so the matrix is invertible
- **Eigenvalues** of `matrix_a`: about 5.54, -2.00 and -0.54
- **Bayes' theorem:** P(Premium | Purchase) = (0.80 × 0.40) / 0.62 ≈ **0.516**
- **Sales data:** mean 165.5, median 165, range 90, sample standard deviation about 23.7
- **Skewness** is about 0.03, so the data is **approximately symmetric**. Excess kurtosis is about -0.71 (flatter than a normal curve).

## Setup: virtual environment

Requires Python 3.9 or newer.

### Windows (PowerShell)

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If PowerShell blocks activation, run `Set-ExecutionPolicy -Scope CurrentUser RemoteSigned` once and try again.

### macOS / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

When the environment is active, `(.venv)` appears at the start of the prompt. Run `deactivate` to leave it.

## Running the notebook

**VS Code:** open the folder, open the notebook, click **Select Kernel**, choose **Python Environments > .venv**, then click **Run All**.

**Browser:**

```bash
jupyter notebook
```

Open `Mathematics_for_Data_Science_Assignment.ipynb` and choose **Kernel > Restart & Run All**.

Random simulations use a fixed seed (`np.random.seed(42)`), so results are reproducible.

## Libraries

NumPy, Pandas, SciPy, Matplotlib, Jupyter, ipykernel.
