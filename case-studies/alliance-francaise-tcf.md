# Inscription Alliance Française / TCF

**Candidate registration and administrative follow-up for TCF-related workflows.**

| Item | Detail |
| --- | --- |
| My roles | Scrum Master, software architect and full-stack developer |
| Team | 4 people |
| First repository commit | 5 October 2024 |
| Latest reviewed commit | 10 September 2026 |
| Stack | PHP 8.2+, Laravel 11, Angular 17, Docker, GitLab CI/CD |
| Public demo | A dedicated registration demonstration is not included yet |

The title is the project name used in this portfolio. It does not claim an official institutional partnership. Dates describe repository history, not a continuous contract.

## Business problem

The registration workflow organizes candidate information, examination data, supporting documents, status follow-up and administrative actions.

## My contribution within the team

I combined Scrum Master responsibilities, software architecture and backend/frontend development within a four-person team.

## Architecture and scope

The relevant implementation includes:

- A Laravel API for candidate and examination workflows.
- An Angular administration application.
- A separate browser extension for form assistance.

The existing repositories also contain unrelated automation. This case study is deliberately limited to candidate registration and administrative follow-up. A future public code sample should extract that scope into a clean demonstration.

## Concrete engineering evidence

- API routes and controllers distinguish candidate, examination, candidate status and identity-document functions.
- The backend dependencies include authentication and permission management.
- Deployment configuration includes application serving and background workers.
- GitLab pipelines automate builds and deployment of the API and administration client.

Pipeline success does not establish registration correctness: the inspected build/deployment pipelines have no business-test gate, and the sampled feature test is the framework's default example.

## Public demonstration scope

A demonstration should show the candidate and administrative workflow using fictitious identities and documents. It should not distribute production records, database exports or the original extension package.

No registration totals or time savings are claimed.

## Next engineering milestones

- Establish a clean registration-only demonstration.
- Add business tests for candidate validation, document handling and status transitions.
- Document permissions and retention of identity documents.
- Reduce the extension's permissions to the sites and actions it actually needs.
- Add screenshots and a short demonstration using synthetic data.

## Interview discussion

I would discuss evolving a long-lived application, separating unrelated product scope, handling sensitive documents and improving quality gates in an existing delivery pipeline.

[Back to the profile](../README.md)

