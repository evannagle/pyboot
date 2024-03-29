# Pyboot

This is a simple python application template for python projects.

Features include:

- Dependency management with [Poetry]()
- Code formatting with [Black]()
- Linting with [Ruff]()
- Unit Testing with [PyTest]()
- Changelog management with []()
- Automation script management with Node and/or Python
- Pre- and post-commit sanity checks with Husky
- Documentation creation with [mkdoc]

## Setup

1. Create a copy of the template

```bash
gh repo create happy-bog --template git@github.com:evannagle/pyboot.git  --private --clone
```

2. Install dependencies

```bash
cd happy-bog

make install
```

3. Rename the app

```bash
make rename
```

4. Run the app

```bash
make app
```

Which should output:

```bash
🤖 Cleaning up
rm -rf __pycache__ .pytest_cache .coverage .mypy_cache .tox .eggs .venv

🤖 Building the project
poetry install
Installing dependencies from lock file

No dependencies to install or update

Installing the current project: pyboot (0.1.0)

🤖 Running the app
poetry run pyboot
42
```

5. Test the app

```bash
make test
```

6. Review test coverage

```bash
make coverage
```

7. Globalize the command for use from your command line

```
make globalize

happy-bog

> 42
```
