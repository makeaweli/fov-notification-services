# FOV Notification Service

A service that notifies satellite operators of upcoming observation schedules and observers of FOV interference alerts.

## Prerequisites

- Python 3.12+
- [uv](https://docs.astral.sh/uv/) (recommended) or pip

## Local Development Setup

### 1. Clone the repository

```bash
git clone https://github.com/iausathub/fov-notification-service.git
cd fov-notification-service
```

### 2. Set up the virtual environment

Using uv (recommended):

```bash
uv venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
uv sync
```

### 4. Set up pre-commit hooks

```bash
pre-commit install
```

This enables automatic code formatting and linting on each commit using:
- **black** - Code formatting
- **ruff** - Linting
- **towncrier** - Changelog management

### 5. Run the application

```bash
python main.py
```

## Development Tools

| Tool | Purpose |
|------|---------|
| black | Code formatter |
| ruff | Linter |
| pre-commit | Git hooks for code quality |
| towncrier | Changelog management |

### Running formatters manually

```bash
# Format code with black
black .

# Lint with ruff
ruff check .

# Auto-fix ruff issues
ruff check --fix .
```

### Running pre-commit on all files

```bash
pre-commit run --all-files
```
