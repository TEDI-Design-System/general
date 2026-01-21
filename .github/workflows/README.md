# Auto Add to Project - Reusable Workflow

This reusable workflow automatically adds issues to a GitHub Project v2 from multiple repositories. It uses an org owned GitHub App for authentication.

## Setup

### Add Caller Workflow to Each Repository

Copy the caller workflow to each repository at `.github/workflows/auto-add-to-project.yml`:

```yaml
name: Auto Add to Project

on:
  issues:
    types:
      - opened
      - transferred

jobs:
  add-to-project:
    uses: TEDI-Design-System/general/.github/workflows/auto-add-to-project.yml@main
    with:
      project-url: https://github.com/orgs/TEDI-Design-System/projects/7
    secrets:
      APP_ID: ${{ secrets.PROJECT_AUTO_ADD_APP_ID }}
      APP_PRIVATE_KEY: ${{ secrets.PROJECT_AUTO_ADD_APP_KEY }}
```

## Customization Options

### Filter by Labels

Add issues only if they have a specific label:

```yaml
jobs:
  add-to-project:
    if: contains(github.event.issue.labels.*.name, 'tedi-ready')
    uses: TEDI-Design-System/general/.github/workflows/auto-add-to-project.yml@main
    # ... rest of config
```

Exclude issues with a specific label:

```yaml
jobs:
  add-to-project:
    if: ${{ !contains(github.event.issue.labels.*.name, 'community') }}
    uses: TEDI-Design-System/general/.github/workflows/auto-add-to-project.yml@main
    # ... rest of config
```

### Different Projects for Different Repositories

Each repository can specify a different `project-url` to add items to different projects.

## Troubleshooting

| Issue | Solution |
|-------|----------|
| **Project not found** | Verify that the project URL is correct |
| **Workflow not found** | Ensure the reusable workflow is in the default branch and the repo is accessible |
| **Token generation failed** | Verify `PROJECT_AUTO_ADD_APP_ID` and `PROJECT_AUTO_ADD_APP_KEY` secrets in org setting are correct |
