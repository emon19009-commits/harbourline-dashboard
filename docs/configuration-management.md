# Configuration management plan

## Configuration items
Pipeline code, database scripts, dashboard files, configuration files (without secrets), test scripts, documentation and the project plan documents.

## Branching
- main: always releasable, protected, no direct pushes
- develop: where finished features are integrated and tested
- feature/DASH-number-short-name: one branch per Jira ticket
- hotfix/...: urgent fixes after go-live

## Commits and reviews
- Commit messages start with the Jira key, so every change traces back to a task or change request
- Every pull request needs at least one approval from another team member before it is merged
- Passwords, keys and connection strings are never committed; they are stored as GitHub Secrets and covered by .gitignore

## Baselines and releases
- Baseline tags at M3 (design approved), M5 (build complete) and M7 (UAT signed off)
- Final release tagged v1.0 at go-live (Week 15)
- Changes to a tagged baseline go through the change request process (see change-log.md)
