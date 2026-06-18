# Assignment 3 - Design Note

Author: Nikhil Kumbhare

## Objective

Implement a reusable GitHub Action that performs lint validation using Maven Checkstyle and blocks pull request merges when linting fails.

## Architecture

1. Custom Action Repository
   - custom-lint-action
   - Contains reusable action.yml

2. Consumer Repository
   - assm-3-spring-petclinic
   - Invokes reusable action during pull requests

## Workflow

Pull Request
→ PR Lint Check Workflow
→ Custom Lint Action
→ Maven Checkstyle
→ Pass / Fail

## Onboarding New Repository

1. Configure Maven Checkstyle.
2. Create PR workflow.
3. Reference the reusable action:
   uses: nikhilk7/custom-lint-action@main

## Benefits

- Reusable across repositories.
- Centralized linting standards.
- Automatic PR validation.
- Prevents non-compliant code from being merged.