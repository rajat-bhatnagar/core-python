# core-python references

The Project uses uv to run python scripts in a lightweight container.

```bash
## Deactivate the currently active environment
# before running uv commands so that uv can create
# and use its own .venv environment cleanly:
(venv) ➜  core-python git:(refactor/rbhatn1/11272025) ✗ deactivate

# IDE currently has a different active venv 
# (like PyCharm's default), uv detects a mismatch 
# and issues this warning.

➜  core-python git:(refactor/rbhatn1/11272025) ✗ uv run main.py
Hello from core-python!


````

## Read
- https://www.python.org

## Code
- https://github.com/fbaptiste/python-blog

## Tools
- https://docs.astral.sh/uv/ - Github Repo (https://github.com/astral-sh/uv)
- PyCharm ( https://www.jetbrains.com/pycharm/ )
  - PyCharm Blog ( https://blog.jetbrains.com/pycharm/ )
  - YT - ( https://www.youtube.com/c/pycharmide )
- Thonny ( https://thonny.org/ ) - brew install thonny