# Assignments for EAPS 507 – Fall 2026

This repository contains my completed Python and Jupyter notebook assignments for EAPS 507 in Fall 2026. It keeps the code, explanations, and required course data together so I can track changes and revisit the analyses.

## Assignments

| Notebook | What it covers |
| --- | --- |
| [Assignment_01_Python_Fundamentals_Madhava_Pi.ipynb](Assignment_01_Python_Fundamentals_Madhava_Pi.ipynb) | Python functions, loops, and lists; approximating pi with the Madhava-Leibniz series; testing different term counts; and plotting convergence and absolute error. |
| [Xarray_10_Minute_Beginner_Tutorial_Completed.ipynb](Xarray_10_Minute_Beginner_Tutorial_Completed.ipynb) | Creating labeled multidimensional weather data with xarray, selecting by position and coordinates, converting temperature units, averaging over named dimensions, and plotting results. |
| [EAPS507_Pandas_Completed.ipynb](EAPS507_Pandas_Completed.ipynb) | Reading pipe-delimited Indiana geographic-feature data; inspecting and filtering records; handling missing values; grouping and aggregating; converting dates; and interpreting and plotting results. |

The descriptive filenames identify each assignment. The pandas notebook is the submitted `EAPS507_3.ipynb` file, renamed here for clarity.

## Run the notebooks

1. Download or clone this repository and open a terminal in its folder.
2. Use Python 3 and install the analysis packages:

   ```sh
   python -m pip install -r requirements.txt
   ```

3. Open the folder in JupyterLab, Jupyter Notebook, VS Code, or another Jupyter-compatible editor. If needed, install and start JupyterLab:

   ```sh
   python -m pip install jupyterlab
   python -m jupyterlab
   ```

4. Select a Python kernel with the required packages installed. Keep `IN_Features_20140204.txt` beside the pandas notebook. Restart the kernel and run the cells from top to bottom.

The pi notebook uses no external data. The xarray notebook creates a small synthetic weather dataset with random seed 42. The pandas notebook reads the included class dataset, `IN_Features_20140204.txt`, using `sep="|"`. The file contains 29,536 geographic-feature records, including 29,417 Indiana records. It is the data file supplied for the course exercise; the original filename is preserved.

## Reproducibility and version history

The notebooks document their methods and interpretations. `requirements.txt` lists the directly used analysis packages; it does not pin an exact environment. Package versions and plotting details can affect results or presentation. A saved notebook output alone does not prove a fresh run succeeded, so rerun from a clean kernel when checking the analysis.

Meaningful commits record additions and documentation changes. A commit identifies a particular snapshot, making it possible to compare changes or return to the code used for an earlier result. When reporting a result, record the commit ID and the Python and package versions used.

Passwords, access tokens, personal files, environment folders, and unnecessary large datasets should stay out of this repository. The `.gitignore` file excludes common secret files and local caches, but notebook cells and outputs should also be reviewed before committing.
