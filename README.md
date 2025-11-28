# core-python references

## Read
- https://www.python.org
- Python Package Index - https://pypi.org/ (Official 3rd party python packages repository)

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
➜  core-python git:(develop) ✗ uv venv py39

Using CPython 3.9.6 interpreter at: /Library/Developer/CommandLineTools/usr/bin/python3
Creating virtual environment at: py39
Activate with: source py39/bin/activate

## Activate the created virtual environment via uv
➜  core-python git:(develop) ✗ source py39/bin/activate 
(py39) ➜  core-python git:(develop) ✗ echo $PATH
/Users/chukku/pycharmProjects/core-python/py39/bin:<OTHER_PATHS>

(py39) ➜  core-python git:(develop) ✗ 

````

## Code
- https://github.com/fbaptiste/python-blog
