# GPM-31: GitHub and Jira Collaboration Rules

## Purpose

These rules explain how the Achievers11-DevOps team uses GitHub and Jira together to deliver the PetClinic project.

## Branch Naming Rule

All branches must follow this format:

feature/GPM-{ticket-number}-{your-name}-{short-description}

Examples:

feature/GPM-226-greg-local-setup
feature/GPM-230-anthonia-aws-deployment-plan
feature/GPM-234-sandra-final-demo
feature/GPM-73-idah-scrum-overdue

## Commit Message Rule

Every commit must reference a Jira ticket number.

Format:

GPM-{number}: description of what was done

Examples:

GPM-31: add GitHub and Jira collaboration rules
GPM-69: create service ownership matrix

## Pull Request Rules

1. Always raise PR from personal fork to Achievers11-DevOps:dev.
2. Never raise PR directly to main.
3. CI must be green before raising PR.
4. At least one reviewer is required.
5. Never merge your own PR.
6. All review comments must be resolved before merge.

## Jira Status Movement Rules

| GitHub Action | Jira Status Moves To |
|--------------|----------------------|
| Branch created with GPM-number | In Progress |
| PR opened referencing GPM-number | In Review |
| PR merged to dev | Done |

## Files Team Members Must Never Modify

- terraform/
- helm/
- argocd/
- docker-compose.yml
- Dockerfile
- pom.xml
- src/
- .github/workflows/ci.yml

## Safe Zones for Team Members

| Area | Purpose |
|------|---------|
| docs/ | Documentation and evidence |
| docs/scrum/ | Scrum coordination documents |
| docs/process/ | Jira and GitHub process documents |
| .github/workflows/{name}-branch-ci.yml | Personal CI workflow only |

## Jira-GitHub Integration

GitHub is connected to Jira using the GitHub for Atlassian app.

Branches, commits, and pull requests automatically appear on Jira tickets when the branch name, commit message, or PR title contains the Jira ticket number.

Example:

GPM-31

## Definition of Done

GPM-31 can be moved to Done when:

- GitHub and Jira collaboration rules are documented.
- Branch naming rules are documented.
- Commit message rules are documented.
- Pull request rules are documented.
- Jira status movement rules are documented.
- This document is committed and pushed to GitHub.
