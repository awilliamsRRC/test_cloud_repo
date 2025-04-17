# Linting Workflow for `dev` Branch

This GitHub Actions workflow automates code linting using [Super-Linter](https://github.com/super-linter/super-linter). It ensures that code meets best practices and maintains consistency across the repository.

## Workflow Overview

- Runs on every `push` and `pull request` targeting the `dev` branch.
- Uses the latest Ubuntu runner (`ubuntu-latest`).
- Performs linting using **Super-Linter** (`v7.3.0`).
- Reports linting results directly to GitHub status checks.

## Configuration

The workflow is defined in `.github/workflows/lint.yml` with the following steps:

1. **Checkout Code** – Retrieves the repository's full git history.
2. **Run Super-Linter** – Executes linting checks on the modified files.

## Usage

To trigger the linter manually:

1. Push changes to the `dev` branch.
2. Open a pull request targeting `dev`.
3. Review linting results under **GitHub Actions** or **Status Checks**.

## Customization

You can modify the linter rules by adjusting the `.github/workflows/lint.yml` file or adding custom configurations via `.super-linter.yml`.

## Learn More

- [Super-Linter Documentation](https://github.com/github/super-linter)
- [GitHub Actions Guide](https://docs.github.com/en/actions)

This workflow helps streamline code quality checks and improve collaboration.
