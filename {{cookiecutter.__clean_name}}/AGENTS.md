# [Project Name]

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
```

## Tech Layers

- **Language**: Python
- **Testing**: Pytest

## Project Structure

```
{{cookiecutter.__clean_slug}}/
├── src/
    ├── {{cookiecutter.__clean_slug}}/          # Main app directory
        ├── {{cookiecutter.__clean_slug}}.py    # App entry point
├── docs/   # App documentation
├── tests/  # App tests
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

### Naming Conventions

- Constants: SCREAMING_SNAKE_CASE

### File Organization

- Group related functions and classes

### Additional Resources
