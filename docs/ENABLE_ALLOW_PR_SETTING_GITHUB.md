# 🔒 Enable Allow-Pull-Request Setting on GitHub

> Refer [CI-BashShell-Formatter-PR](https://github.com/pnguyen215/shell-devops-stores/blob/master/ci-cd/github-actions/ci-bashshell-formatter-pr.yml)

```yaml
# Permissions for the workflow
# This workflow requires write permissions to contents and pull requests
permissions:
  contents: write # allows modifying files
  pull-requests: write # allows creating/updating PRs
```

Go to **Settings** → **Actions** → **General** for the repository:

- Ensure "**Workflow permissions**" is set to "**Read and write permissions**" or use the toggle.
- Then check "**Allow GitHub Actions to create and approve pull requests**"

If this checkbox is greyed out, it's likely managed at the organization or enterprise level. In that case, ask your org admin to enable it under **Organization Settings** → **Actions** → **General** first, then enable it at the repo level.
