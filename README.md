# virtual-environments
Yaml files for virtual environment - Coppied from NCIL_data_science_environments; see LISCENCE

These configuration files will allow you to create dedicated environments (sets of Python and R packages) for typical NCIL use cases. 

The environments:
- `ncil.yml`: Python environment for data science, including Jupyter Lab, pandas, numpy, matplotlib, seaborn, scikit-learn, and more.

To use, clone this repository to your computer, or just download the individual file you want. Then in a terminal window (**on Windows this *must* be a Conda or Miniforge Terminal**), `cd` to the folder containing this repository and run:
```
mamba env create -f ncil.yml
```

(or whatever the name of the file is).

This will install all the packages into a dedicated environment. When you want to use it, in a terminal run:
```
mamba activate ncil
```
Then proceed as usual (e.g., run `jupyter lab`). 

If you are using VS Code, you don't need to run `mamba activate`. Instead, when you open a Python file or notebook be sure to select the `ncil` environment in the upper right corner (rather than the default `base` environment).
