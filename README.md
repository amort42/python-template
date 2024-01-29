# python-template

Template for python-based repositories.

## Usage

1. Use this repository by specifying it as a template for your repository.
2. run `./script/bootstrap`

## Notes for personal setup
(from https://armandsauzay.medium.com/python-project-setup-a-step-by-step-guide-to-industry-best-practices-dbce717b2d12)
1. gh repo create amort42/hello-world-cli --template amort42/python-template --public
2. git clone https://github.com/amort42/hello-world-cli.git
3. cd hello-world-cli
4. ./script/bootstrap
5. Using pyenv and poetry
    1. pyenv install <version>
    2. pyenv global <version>
    3. pip install poetry
    4. poetry add requests mypy
    5. poetry add --group lint flake8 black isort **mypy**
    6. poetry run pytest
    7. poetry run mypy hello_world_cli/main.py
    8. poetry run flake8 hello_world_cli/cli.py
    9. poetry run black hello_world_cli/cli.py
