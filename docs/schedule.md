# Project schedule (baseline)

All dependencies are finish-to-start.

| ID | Task | Duration | Weeks | Predecessors | Owner |
|---|---|---|---|---|---|
| T1 | Initiation and charter | 1 wk | 1 | None | PM |
| T2 | Requirements gathering | 2 wks | 2-3 | T1 | BA/QA |
| T3 | Data source audit | 2 wks | 2-3 | T1 | Dev |
| T4 | Architecture and data model design | 2 wks | 4-5 | T2, T3 | Dev |
| T5 | Dashboard wireframes | 2 wks | 4-5 | T2 | BA/QA |
| T6 | Environment and repository setup | 2 wks | 2-3 | T1 | Dev |
| T7 | Data pipeline build | 3 wks | 6-8 | T4, T6 | Dev |
| T8 | Reporting database build | 2 wks | 6-7 | T4, T6 | Dev |
| T9 | Dashboard development | 3 wks | 8-10 | T5, T8 | Dev |
| T10 | Security and access control | 2 wks | 9-10 | T7 | Dev |
| T11 | Integration testing | 2 wks | 11-12 | T7, T9 | BA/QA |
| T12 | Security and performance testing | 2 wks | 11-12 | T9, T10 | BA/QA |
| T13 | User acceptance testing | 2 wks | 13-14 | T11, T12 | BA/QA |
| T14 | Training and documentation | 4 wks | 11-14 | T9 | BA/QA |
| T15 | Deployment and go-live | 1 wk | 15 | T13, T14 | PM |
| T16 | Hypercare, handover and closure | 1 wk | 16 | T15 | PM |
| T17 | Project management and reporting | 16 wks | 1-16 | None | PM |

## Milestones

| Milestone | End of week |
|---|---|
| M1 Charter approved | 1 |
| M2 Requirements signed off | 3 |
| M3 Design approved | 5 |
| M4 Pipelines and reporting database complete | 8 |
| M5 Dashboard build complete | 10 |
| M6 Testing complete | 12 |
| M7 UAT signed off | 14 |
| M8 Go-live | 15 |
| M9 Project closed | 16 |

## Critical path

T1 > T2/T3 > T4 > T8 > T9 > T11 > T13 > T15 > T16, and T4 > T7 > T10 > T12 > T13.
Only T5 and T6 have slack (about two weeks each).
