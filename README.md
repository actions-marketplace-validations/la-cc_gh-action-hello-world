# Introduction

This is simple example of GitHub Action that will be published to GitHub Marketplace.

## Usage

```
name: hello-world-example-101-101

on:
  workflow_dispatch:
  push:
    branches:
      - main
    paths:
      - ".github/workflows/test-hello-world.yml"

jobs:
  hello-world-example:
    name: "Test: Hello World 101-101"
    runs-on: ubuntu-latest
    steps:
      - name: Hello World 101-101
        uses: la-cc/gh-action-hello-world@v0.0.3
        with:
          custom-text: "Hi, my name is 101-101!"
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
