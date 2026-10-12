# Target4C2

**A training and TCF preparation platform with separate identity, learning and enrollment domains.**

| Item | Detail |
| --- | --- |
| My roles | Scrum Master, software architect and full-stack developer |
| Team | 4 people |
| First repository commit | 11 August 2026 |
| Latest reviewed commit | 21 August 2026 |
| Stack | Java 25, Spring Boot 4.0.7, Angular 21, PostgreSQL, Flyway, Docker |
| Demo link | [Target4C2](https://target4c2.mybestsejour.com/) |
| Availability at review | The public link returned 502 on 10 October 2026 |

These dates describe repository history. The demonstration link needs restoration before it can support an interview.

## Business problem

The product structures TCF preparation and training around learner accounts, learning content, pedagogy, enrollment and learner access.

## My contribution within the team

My roles covered Scrum Master responsibilities, software architecture and full-stack implementation in a four-person team.

## Architecture

The repository contains eight services:

- Config service, discovery service and API Gateway.
- Identity and access.
- Public CMS and marketing.
- Learning content.
- Training and pedagogy.
- Commerce operations.

The Angular client integrates with API contracts. Identity uses JWT resource-server configuration; database migrations describe enrollment, payment and offer data.

## Concrete engineering evidence

- The backend is separated by identity, content, training and commercial responsibilities.
- Docker builds produce service images tagged with the commit.
- The deployment uses Docker Compose and configuration variables.
- Enrollment and learner access have explicit states such as pending payment, locked and active.

## Payment scope

The reviewed payment flow is a **demonstration implementation**. Checkout URLs are simulated and a demonstration action marks a payment as paid. This case study does not claim a completed Stripe integration or verified processing of real payments.

A production payment milestone must include provider verification, server-controlled pricing, ownership checks and protected activation of access.

## Validation status

The recorded backend build/deployment succeeded. The inspected Docker build skips Maven tests. Backend test scaffolding exists, but this review did not establish a business-test gate.

No live enrollment or payment was performed during the audit.

## Next engineering milestones

- Restore the public demonstration.
- Keep simulated payment actions confined to a controlled demonstration environment.
- Complete and test payment-provider confirmation and ownership controls.
- Add business tests for enrollment, payment failure and access activation.
- Add frontend tests and a documented local environment.

## Interview discussion

I would explain the domain boundaries and delivery pipeline, then distinguish completed architecture work from the payment integration and reliability work still required.

[Back to the profile](../README.md)

