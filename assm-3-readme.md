# Custom Lint Action

Author: Nikhil Kumbhare

## Overview

This reusable GitHub Action executes Maven Checkstyle validation.

## Usage

```yaml
- name: Run Custom Lint Action
  uses: nikhilk7/custom-lint-action@main
```

## Result

- Passes when no lint violations exist.
- Fails when Checkstyle violations are detected.
- Can be reused across multiple repositories.