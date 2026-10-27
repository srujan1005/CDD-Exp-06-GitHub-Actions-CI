# CDD Lab Experiment 6: Continuous Integration with GitHub Actions

## Objective
Create Continuous Integration workflows using GitHub Actions.

## Duration
2 Hours

## Tasks
1. Create a `.github/workflows` directory.
2. Write a basic CI workflow YAML file.
3. Trigger the workflow on push or pull request.
4. Add steps for checkout, setup, and a simple test/build.
5. Monitor the workflow run in the Actions tab.

## Sample Workflow
```yaml
name: CI
on: [push, pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run a simple script
        run: echo "CI workflow is running"
```

## Expected Outcome
A working GitHub Actions CI workflow that runs successfully.
