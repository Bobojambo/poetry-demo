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