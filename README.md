# Commitizen Demo

> **Note:** This repository is for **testing and demonstration purposes only**. It showcases customized Commitizen commit message configurations and examples.

## Purpose

This repo demonstrates how to customize Commitizen commit messages to create structured, standardized commit history without the default SemVer/CI tool examples.

## Available Commit Types

The following commit types are configured in [pyproject.toml](pyproject.toml):

- **fix** - Bug fix
- **feat** - New feature
- **docs** - Documentation changes
- **style** - Code formatting (no logic change)
- **refactor** - Code restructuring
- **perf** - Performance improvement
- **test** - Add or update tests
- **build** - Build system or dependencies
- **ci** - CI/CD configuration
- **chore** - Maintenance tasks
- **revert** - Revert previous commit

## Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Examples

```
feat: add user authentication

docs: update README with setup instructions

fix(api): resolve timeout issue in user endpoint

refactor: simplify error handling logic

The error handling was spread across multiple functions.
Consolidated into a single utility module for better maintainability.

Closes #123
```

## Usage

1. Stage your changes: `git add .`
2. Run commitizen: `cz commit`
3. Follow the interactive prompts
4. Your commit message is automatically formatted

## Configuration

All customization is defined in the `[tool.commitizen.customize]` section of [pyproject.toml](pyproject.toml).