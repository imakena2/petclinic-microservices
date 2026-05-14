# GPM-126: GitHub Repository Access Confirmation

## Purpose

This document confirms GitHub repository access for the Achievers11-DevOps PetClinic project team.

The goal is to ensure every team member can access the required repositories, work from their fork, create feature branches, and raise pull requests to the team dev branch.

## Organisation

Achievers11-DevOps

## Repositories

| Repository | Purpose |
|-----------|---------|
| petclinic-microservices | Application source code and documentation |
| petclinic-k8s-platform | Infrastructure, Kubernetes, Helm, and ArgoCD platform work |

## Team Member Access Status

| Team Member | GitHub Username | Access Status | Responsibility |
|------------|----------------|---------------|----------------|
| Osenat Alonge | etaoko333 | Confirmed | Infrastructure and platform |
| Greg | gregodprogrammer | Confirmed | Technical lead and architecture |
| Sandra | sandraolis | Confirmed | Presentation and demo evidence |
| Anthonia | adekunleanthonia632-alt | Confirmed | AWS and deployment documentation |
| Idah Makena | imakena2 | Confirmed | Scrum Master and Jira Lead |

## Access Requirements

Each team member should be able to:

- View the organisation repositories
- Fork the repositories to their own GitHub account
- Clone their fork locally
- Add the organisation repository as upstream
- Create feature branches
- Push changes to their personal fork
- Raise pull requests to Achievers11-DevOps:dev

## Standard Working Flow

1. Fork the organisation repository.
2. Clone the personal fork locally.
3. Add the organisation repository as upstream.
4. Create a feature branch from main.
5. Make changes only in the allowed files or folders.
6. Commit using the Jira ticket number.
7. Push to the personal fork.
8. Raise a pull request to the dev branch.

## Pull Request Target Rule

All pull requests must target:

Achievers11-DevOps/petclinic-microservices:dev

Team members must not raise pull requests directly to main.

## Definition of Done

GPM-126 can be moved to Done when:

- Team member GitHub usernames are documented
- Repository access expectations are documented
- Fork and branch workflow is documented
- Pull request target branch is documented
- This document is committed and pushed to GitHub
