# {{cookiecutter.__clean_slug}}

{{cookiecutter.project_description}}

## Development Setup

```bash
# Installation
uv sync

# Lint
task lint

# Format
task format

# Run
task run

# Tests
task tests

# Test Coverage
task coverage

# Run tests via nox
task nox
```

## Tech Layers

- **Language**: Python 3.11+
- **Package Manager**: uv
- **Testing**: pytest, pytest-cookies
- **Linting**: ruff

## Project Structure

```
{{cookiecutter.__clean_slug}}/
├── src/                                        # App source code
    ├── {{cookiecutter.__clean_slug}}/          # Main app directory
        ├── {{cookiecutter.__clean_slug}}.py    # App entry point
├── docs/                                       # App documentation
├── tests/                                      # App tests
└── pyproject.toml                              # Project config
```

## Development Guidelines

### Key Principles

- DO: Prioritize readability and maintainability
- DO: Write tests for new features
- DO: Check existing functions before creating new ones
- DO: Follow established patterns in the codebase
- DO: Keep functions small and focused
- DO: Include typehinting for all created code
- DON'T: Create new files unless necessary
- DON'T: Skip tests for "simple" features

### Testing Approach

- All tests go in the `tests/` directory following the project structure
- Tests should be runnable with `task tests` or `uv run pytest tests/`

### Naming Conventions

- Constants: `SCREAMING_SNAKE_CASE`
- Functions/variables: `snake_case`
- Classes: `PascalCase`

### File Organization

- Group related functions and classes
- Files live in `{{cookiecutter.__clean_name}}/`

### Safety and permissions

Allowed without prompt:

- read files, list files
- python single file, linting, formatting,
- pytest single test

Ask first:

- package installs,
- git push
- deleting files, chmod
- running full build or end to end suites

### When stuck

- ask a clarifying question, propose a short plan, or open a draft PR with notes
- do not push large speculative changes without confirmation
