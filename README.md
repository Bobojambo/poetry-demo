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