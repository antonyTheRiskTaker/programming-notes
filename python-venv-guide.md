### How to set a virtual environment using venv?
A: type `python3 -m venv <name of the venv directory>` inside your project
directory.
**N.B. you cannot specify what Python version you want**

### How to activate a virtual environment?
Step 1: `cd <name of the project directory>/`
step 2: `source <name of the venv directory>/bin/activate`

### How to exit a virtual environment?
A: type `deactivate`.

### How to remove a virtual environment>
A: type `rm -rf <name of venv directory>/` in the directory where the
virtual environment is stored.

### How to export the packages that you're using for a specific environment?
A: This can be done with a `requirements.txt` file, which allows someone else
to create an enviroment and use your `requirements.txt` file to install all of
the packages and dependencies of the same versions that you're using.
Steps:
  1. run the `pip freeze > requirements.txt` command.
  2. run the `pip install -r requirements.txt` to install packages.