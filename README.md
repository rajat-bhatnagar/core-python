# core-python references

## Read
- https://www.python.org
- Python Package Index - https://pypi.org/ (Official 3rd party python packages repository)
- PEP Style guide - https://peps.python.org
- Python Operator Precedence - https://docs.python.org/3/reference/expressions.html#operator-precedence

## Tools
- https://docs.astral.sh/uv/ - Github Repo (https://github.com/astral-sh/uv)
- PyCharm ( https://www.jetbrains.com/pycharm/ )
  - PyCharm Blog ( https://blog.jetbrains.com/pycharm/ )
  - YT - ( https://www.youtube.com/c/pycharmide )
- Thonny ( https://thonny.org/ ) - brew install thonny


The Project uses uv to run python code.
```bash
## Deactivate the currently active environment
# before running uv commands so that uv can create
# and use its own .venv environment cleanly:
(venv) ➜  core-python git:(develop) ✗ deactivate

# IDE currently has a different active venv 
# (like PyCharm's default), uv detects a mismatch 
# and issues this warning.

➜  core-python git:(develop) ✗ uv run main.py
Hello from core-python!

## Create a new virtual environment with uv
➜  core-python git:(develop) ✗ uv venv .venv

Using CPython 3.9.6 interpreter at: /Library/Developer/CommandLineTools/usr/bin/python3
Creating virtual environment at: .venv
Activate with: source .venv/bin/activate

## Activate the created virtual environment via uv
➜  core-python git:(develop) ✗ source .venv/bin/activate 
(.venv) ➜  core-python git:(develop) ✗ echo $PATH
/Users/chukku/pycharmProjects/core-python/.venv/bin:<OTHER_PATHS>

(.venv) ➜  core-python git:(develop) ✗ 

# add and install a runtime package (writes/updates `uv.lock`)
uv add requests
# specify a version
uv add requests==2.31.0

# add a dev dependency
uv add pytest --dev

# install all packages from `uv.lock`
uv install

# remove a package
uv remove requests

# upgrade a package
uv upgrade requests

# IMPORTANT:
# If you use uv commands that manage packages (for example uv add, uv remove, uv upgrade)
# they update uv.lock automatically and install into the venv. 
# If you install with pip directly, uv.lock will not be updated
# — run 
uv sync 
# to reconcile the lockfile and environment.


# Added additional packages 

➜  core-python git:(develop) ✗ uv venv .venv
#Using CPython 3.9.6 interpreter at: /Library/Developer/CommandLineTools/usr/bin/python3
#Creating virtual environment at: .venv

➜  core-python git:(develop) ✗ source .venv/bin/activate

(.venv) ➜  core-python git:(develop) ✗ uv add notebook pytz python-dateutil requests openpyxl xlrd pip jupyterthemes
#warning: `VIRTUAL_ENV=.venv` does not match the project environment path `.venv` and will be ignored; use `--active` to target the active environment instead
#Using CPython 3.9.6 interpreter at: /Library/Developer/CommandLineTools/usr/bin/python3
#Creating virtual environment at: .venv
#Resolved 116 packages in 682ms
#Prepared 101 packages in 3.08s
#Installed 102 packages in 237ms

# Generated the requirements.txt file using uv

(.venv) ➜  core-python git:(develop) ✗ uv run pip freeze > requirements.txt

#List available jupyter themes
(.venv) ➜  core-python git:(develop) ✗ jt -l

# Select the Dark theme
(.venv) ➜  core-python git:(develop) ✗ jt -t onedork

````

## Code
- https://github.com/fbaptiste/python-blog
