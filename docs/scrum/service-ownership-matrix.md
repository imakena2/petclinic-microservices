# GPM-69: Service Ownership Matrix

## Purpose

This document defines ownership responsibilities for the Achievers11-DevOps PetClinic microservices project.

The goal is to make it clear who owns each area of the project and who should be contacted when support or escalation is needed.

## Infrastructure and Platform Ownership

| Resource | Owner | GitHub Username | Responsibility |
|----------|-------|----------------|----------------|
| AWS EKS cluster | Osenat Alonge | etaoko333 | Provision and maintain cluster |
| Terraform modules | Osenat Alonge | etaoko333 | Write and apply infrastructure code |
| Helm charts | Osenat Alonge | etaoko333 | Maintain Kubernetes deployment charts |
| ArgoCD | Osenat Alonge | etaoko333 | Configure and monitor GitOps deployment |
| ECR repositories | Osenat Alonge | etaoko333 | Manage container image repositories |
| RDS MySQL | Osenat Alonge | etaoko333 | Provision and maintain database |
| AWS Secrets Manager | Osenat Alonge | etaoko333 | Store and manage secrets |
| Main CI/CD pipeline | Osenat Alonge | etaoko333 | Own main deployment pipeline |

## Application Architecture and Documentation Ownership

| Deliverable | Owner | GitHub Username | Responsibility |
|-------------|-------|----------------|----------------|
| Architecture documentation | Greg | gregodprogrammer | Own technical architecture documents |
| Local setup documentation | Greg | gregodprogrammer | Document local setup process |
| Code review process | Greg | gregodprogrammer | Define review rules and PR standards |
| Technical guidance | Greg | gregodprogrammer | Support technical decisions |

## AWS and Deployment Documentation Ownership

| Deliverable | Owner | GitHub Username | Responsibility |
|-------------|-------|----------------|----------------|
| AWS documentation | Anthonia | adekunleanthonia632-alt | Support AWS documentation |
| Deployment notes | Anthonia | adekunleanthonia632-alt | Document deployment-related steps |
| Cloud evidence | Anthonia | adekunleanthonia632-alt | Support AWS evidence collection |

## Presentation and Demo Ownership

| Deliverable | Owner | GitHub Username | Responsibility |
|-------------|-------|----------------|----------------|
| Presentation slides | Sandra | sandraolis | Compile and present final slides |
| Demo script | Sandra | sandraolis | Prepare and rehearse demo script |
| Evidence screenshots | Sandra | sandraolis | Capture and organise screenshots |
| Non-technical walkthrough | Sandra | sandraolis | Explain the project clearly to audience |

## Scrum and Jira Ownership

| Deliverable | Owner | GitHub Username | Responsibility |
|-------------|-------|----------------|----------------|
| Jira project management | Idah Makena | imakena2 | Manage Jira board and tickets |
| Sprint planning | Idah Makena | imakena2 | Facilitate and document sprint planning |
| Blocker tracking | Idah Makena | imakena2 | Track and escalate blockers |
| GitHub-Jira integration | Idah Makena | imakena2 | Document integration process |
| Bug tracking process | Idah Makena | imakena2 | Define bug reporting and tracking process |
| Scrum documentation | Idah Makena | imakena2 | Maintain Scrum process documents |

## Escalation Matrix

| Issue Type | First Contact | Escalate To |
|-----------|---------------|-------------|
| AWS or infrastructure issue | Osenat | Greg |
| Code or architecture issue | Greg | Osenat |
| Jira or process issue | Idah | Greg |
| Presentation issue | Sandra | Idah |
| Blocker affecting delivery | Idah | Greg and Osenat |
| Deployment issue | Osenat | Greg |

## Definition of Done

GPM-69 can be moved to Done when:

- Team ownership areas are documented
- Infrastructure ownership is documented
- Scrum and Jira ownership is documented
- Presentation ownership is documented
- Escalation matrix is documented
- This document is committed and pushed to GitHub
