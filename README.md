# Harbourline Real-Time Analytics Dashboard

Configuration management repository for the Harbourline Retail Group dashboard project (Jira project key: **DASH**).
Harbourline Retail Group is a fictional retailer used for our university project plan.

## About the project

Harbourline has 14 stores and an online shop. Sales, stock and website data sit in three separate systems and reports are a week old.
This project builds a cloud dashboard that pulls data from the point-of-sale (POS), e-commerce and inventory systems and shows it to managers within about 60 seconds.

- Duration: 16 weeks
- Budget: AUD 158,400 (including 10% contingency)
- Dashboard areas: Sales, Inventory, Online Performance

## Repository structure

| Folder | Contents |
|---|---|
| `docs/` | Project plan, schedule, risk register, change log and design documents |
| `pipelines/` | Data pipeline code for the POS, e-commerce and inventory systems |
| `database/` | Reporting database scripts (dimensional model) |
| `dashboard/` | Dashboard files for the three dashboard areas |
| `tests/` | Integration, security, performance and UAT test scripts |
| `config/` | Configuration files (never passwords, keys or connection strings) |

## Branches

- `main`: always releasable, changed only through pull requests
- `develop`: finished features are combined and tested here
- `feature/DASH-<number>-short-name`: one branch per Jira task
- `hotfix/...`: urgent fixes after go-live

## Rules

- Every commit message starts with its Jira key, for example `DASH-23: add low-stock tile to inventory page`
- Every pull request is reviewed by another team member before it is merged
- Passwords, keys and connection strings are never committed; they are kept in GitHub Secrets
- Baselines are tagged at Milestones M3, M5 and M7, and the final release is tagged v1.0 at go-live
