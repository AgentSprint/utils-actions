# utils-actions

This repository contains custom GitHub Actions designed to automate and enhance workflows for your projects. Each action is built to be reusable and easy to integrate into your CI/CD pipelines.

## Repository Structure

- `main.py` — Main script for utility functions or orchestration.
- `pyproject.toml` — Python project configuration and dependencies.
- `comment-on-issue/` — Contains the `comment-on-issue` GitHub Action.
  - `action.yml` — Metadata and configuration for the action.

## Available Actions

### comment-on-issue
Adds a comment to a specified GitHub issue. Useful for automating notifications, status updates, or feedback in your workflow.

**Usage Example:**
```yaml
- name: Comment on Issue
  uses: AgentSprint/utils-actions/comment-on-issue@main
  with:
    issue-number: 123
    comment: "This is an automated comment."
    github-token: ${{ secrets.GITHUB_TOKEN }}
```

## How to Use
1. Reference the desired action in your workflow YAML file using the `uses` keyword.
2. Provide required inputs as specified in the action's documentation (`action.yml`).
3. Make sure to use a valid GitHub token for authentication when required.

## Contributing
Feel free to open issues or pull requests to add new actions or improve existing ones. Contributions are welcome!

## License
This repository is licensed under the MIT License.
