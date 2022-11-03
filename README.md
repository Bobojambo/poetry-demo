# Add dependency with poetry
poetry add pendulum

pip install virtualenv 
virtualenv .venv
.\.venv\Scripts\activate
poetry env info --path

# Activating virtual env in poetry
`& ((poetry env info --path) + "\Scripts\activate.ps1")`
## activate poetry shell
`poetry shell`
## exit shell
`exit`

## Information about poetry environment installation and upate
https://python-poetry.org/docs/basic-usage/

## Project uses mlops 
https://www.mlflow.org/docs/latest/quickstart.html

## Configuring posh-git for windows
Import-Module posh-git # Needs to be run everytime in new powershell
configure better at:
https://computingforgeeks.com/posh-git-powershell-environment-for-git/

## Python dependencies for devops
- Poetry for managing dependencies and packaging
- pre-commit for running all the goodies listed below
- mypy for static type checking
- flake8 (with multiple plugins) for linting (e.g. style and complexity checks, commented code, etc.)
- black for auto-formatting the code
- isort for auto-sorting imports
- sautoflake for auto-removing unused imports

## Errors with conda and windows
CondaHTTPError: HTTP 000 CONNECTION FAILED for url <https://repo.anaconda.com/pkgs/main/win-64/current_repodata.json>

What worked for me is
conda config --set ssl_verify False
and then I run conda update conda

- Conda in powershell
  - https://gist.github.com/martinsotir/2bd2e16332dff71e0fa5be3ed3468a6c
  - conda init powershell

conda create -n myenv python=3.9
