# copier-cli

[Copier](https://github.com/copier-org/copier) template for Python CLIs with [Click](https://click.palletsprojects.com/en/8.1.x/) and [Poetry](https://python-poetry.org/).

## Quickstart

```bash
copier "gh:joaopalmeiro/copier-cli" <cli_name>
```

## Development

- `export PIPENV_VENV_IN_PROJECT=1 && pipenv install --python 3.7`
- `pipenv run copier --version`
- `pipenv run djlint project/* --lint --profile=jinja`
- `rm -rf demo && pipenv run copier . demo` or `rm -rf demo && pipenv run copier "gh:joaopalmeiro/copier-cli" demo`

## Deployment

- After finishing a new template version, [create a new release in the GitHub repository](https://github.com/joaopalmeiro/copier-cli/releases)

## Notes

- [Copier](https://github.com/copier-org/copier):
  - [Documentation](https://copier.readthedocs.io/en/latest/)
  - [pdm-project/copier-pdm](https://github.com/pdm-project/copier-pdm) template
  - [pawamoy/copier-pdm](https://github.com/pawamoy/copier-pdm) template
  - [pawamoy/copier-poetry](https://github.com/pawamoy/copier-poetry) template
  - Install: `pipx install copier`
- ['save-exact' option for saving exact version in Pipfile](https://github.com/pypa/pipenv/issues/3441) (open) issue
- [djLint](https://djlint.com/):
  - [Linter](https://djlint.com/docs/linter/)
  - [VS Code extension](https://marketplace.visualstudio.com/items?itemName=monosans.djlint)
  - `pipenv run djlint project/* --check --profile=jinja`
  - `pipenv run djlint project/* --reformat --profile=jinja`
  - `pipenv run djlint project/\{\{_copier_conf.answers_file\}\}.jinja --reformat --profile=jinja`
- GitHub topics ([source](https://github.com/topics/copier-template)):
  - python
  - template
  - scaffolding
  - bootstrapping
  - copier
  - copier-template
