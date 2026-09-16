# GitHub Actions

This repository contains GitHub Actions workflows for automating project tasks.

## Usage

1. Add workflow files to `.github/workflows/`.
2. Configure the workflow triggers, jobs, and steps.
3. Commit and push the changes to GitHub.

GitHub will run the workflows automatically when their configured events occur.

## Example

```yaml
name: CI

on:
	push:
		branches: [main]
	pull_request:

jobs:
	build:
		runs-on: ubuntu-latest
		steps:
			- uses: actions/checkout@v4
			- run: echo "Workflow completed successfully"
```

## License

MIT
