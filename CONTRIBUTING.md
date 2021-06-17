# Contributing Guide

This doc covers dev setup and guidelines for contributing.

FIXME: This doc is a stub.

## Requirements

- python3.7+ (prefer 3.7), pip, virtualenv
- docker

### Recommended

- [pipx](https://pypa.github.io/pipx/)
- [pre-commit](https://pre-commit.com/)

You can install `pipx` first, and then use it to install other tools, as in

    pipx install pre-commit

## Linting & Testing

Testing should be done in a virtualenv with pytest. Setup:

    pip install -r ./requirements.txt
    pip install -r ./requirements_test.txt

Run tests with

    pytest

Linting can be run via pre-commit. Run for all files in the repo:

    pre-commit run -a

### (Optional) Setup pre-commit Hooks

For the best development experience, set up linting and autofixing pre-commit
git hooks using the `pre-commit` tool.

After installing `pre-commit`, run

    pre-commit install

in the repo to configure hooks.

> NOTE: If necessary, you can always skip hooks with `git commit --no-verify`
