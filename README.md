# PiBrewing Workflows

This repository contains reusable workflows to be used within the PiBrewing community.

## Usage example

Within your repo create a file called `.github/workflows/ci.yaml` with the following content:

```yaml
on:
  push: ["main"]
jobs:
  lint-and-test:
    uses: PiBrewing/workflows/.github/workflows/ci-python.yaml
```

This will enable a workflow which lints and tests your python code on every push to the mai branch
using the reusable workflow from this repository.

## Available workflows

* ci-python.yaml: A simple workflow which lints and tests a python project
