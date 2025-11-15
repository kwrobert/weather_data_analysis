# Weather Data Analysis

A modern Python project for weather data analysis.

## Prerequisites

- [mise](https://mise.jdx.dev/) - Runtime and tool version manager
- [uv](https://github.com/astral-sh/uv) - Fast Python package manager

## Setup

1. Install mise and uv if you haven't already:
```bash
# Install mise
curl https://mise.run | sh

# Install uv
curl -LsSf https://astral.sh/uv/install.sh | sh
```

2. Install Python and create virtual environment:
```bash
mise install
```

This will automatically:
- Install Python 3.12
- Create a virtual environment at `.venv`

3. Install project dependencies:
```bash
mise run install
# or manually: uv sync
```

## Development

### Available Tasks

Run tasks using `mise run <task>`:

- `mise run install` - Install project dependencies
- `mise run test` - Run tests with pytest
- `mise run lint` - Run linting checks with ruff
- `mise run format` - Format code with ruff
- `mise run type-check` - Run type checking with mypy

### Project Structure

```
.
├── mise.toml              # mise configuration and tasks
├── pyproject.toml         # Python project configuration
├── .python-version        # Python version specification
├── src/
│   └── weather_data_analysis/
│       └── __init__.py    # Main package
└── tests/
    ├── __init__.py
    └── test_example.py    # Example tests
```

## Running Tests

```bash
mise run test
```

## Code Quality

Format code:
```bash
mise run format
```

Run linting:
```bash
mise run lint
```

Run type checking:
```bash
mise run type-check
```
