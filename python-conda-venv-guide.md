### To create a requirements.txt from a conda venv:
A: Please also reference this stackoverflow page: 
https://stackoverflow.com/questions/50777849/from-conda-create-requirements-txt-for-pip3
  1. Enter a conda virtual environment.
  2. Run this command: `pip list --format=freeze > requirements.txt`.

### To update conda:
A: Run `conda update conda`.

### To check available Python versions for venv:
A: Run `conda search python`.

### To list all known conda environments:
A: Run `conda info -e` or `conda info --envs`.

### To create a new conda venv (specifying Python version):
A: Run `conda create -n ENV_NAME python=PY_VER`, e.g. `python=3.9`.

### To remove a conda venv:
A: Run `conda remove -n ENV_NAME --all`.

### To activate a conda venv:
A: Run `conda activate ENV_NAME`.

### To exit a conda venv:
A: Run `conda deactivate`.