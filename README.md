# [Level up program](https://github.com/minaeiehsan/level-up) demo project: **PYTHON**

> **ATTENTION**

This code is focused to demonstrate TED (Test driven development, Event driven architecture and Domain driven Design) topics in level up program, to make it concise some basic stuff is dropped intentionally (e.g hard coded config) or resolving dependencies might be questionable. feel free to ask about best practices during the workshop.

## Requirements

- Docker
- A local python3.8+

## Building the containers

```sh
make build
make up
# or
make all # builds, brings containers up, runs tests
```

## Creating a local virtualenv (optional)

```sh
python3.8 -m venv .venv && source .venv/bin/activate # or however you like to create virtualenvs

pip install pytest

pip install pytest sqlalchemy

pip install -r requirements.txt

pip install -r requirements.txt
pip install -e src/
```

## Running the tests

```sh
make test
# or, to run individual test types
make unit
make integration
make e2e
# or, if you have a local virtualenv
make up
pytest tests/unit
pytest tests/integration
pytest tests/e2e
```

## Makefile

There are more useful commands in the makefile, have a look and try them out.
