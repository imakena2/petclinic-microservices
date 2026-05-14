# GPM-189: Create, Manage and Track Bugs in Jira and GitHub

## Purpose

This document explains how the Achievers11-DevOps team creates, manages, tracks, and closes bugs using Jira and GitHub.

The goal is to make sure every bug is clearly reported, assigned, fixed, reviewed, and closed.

## Bug Lifecycle

Open -> In Progress -> In Review -> Resolved -> Closed

## How to Create a Bug in Jira

1. Go to the Jira GPM project.
2. Click Create.
3. Select Issue type: Bug.
4. Add a short and clear summary.
5. Add a detailed description.
6. Add steps to reproduce the bug.
7. Add the expected result.
8. Add the actual result.
9. Set the correct priority.
10. Add the correct label.
11. Assign the bug to the person responsible.
12. Click Create.

## Bug Report Template

Summary: [Short description of the bug]

Environment: Local / Docker Compose / AWS EKS

Steps to reproduce:
1. Step one
2. Step two
3. Step three

Expected result:
What should happen.

Actual result:
What actually happened.

Error message:
Paste the exact error message, if available.

Resolution:
Explain how the bug was fixed after the fix is complete.

## Bug Priority Guide

| Priority | Meaning | Example |
|----------|---------|---------|
| Highest | The application is completely down | EKS cluster not responding |
| High | A major feature is broken | Database connection failing |
| Medium | A feature is degraded but workaround exists | Grafana showing no data |
| Low | Minor issue or warning | Non-blocking warning in logs |

## Bug Labels

Use these labels to make bugs easier to search and manage:

| Label | When to Use |
|-------|-------------|
| docker | Docker or Docker Compose issues |
| aws | AWS infrastructure issues |
| terraform | Terraform provisioning issues |
| monitoring | Prometheus, Grafana, or Zipkin issues |
| ci-cd | GitHub Actions or deployment pipeline issues |
| documentation | Documentation errors or missing information |

## Linking Bugs to GitHub

When fixing a bug, create a GitHub branch using this format:

feature/GPM-{bug-number}-{name}-fix-{short-description}

Example:

feature/GPM-107-idah-fix-docker-container-conflict

## Commit Message Rule

Every bug fix commit must include the Jira ticket number.

Example:

GPM-107: fix Docker container conflict documentation

## Pull Request Rule

Every bug fix PR title must include the Jira ticket number.

Example:

GPM-107: fix Docker container conflict documentation

This helps Jira automatically link the GitHub branch, commit, and pull request to the correct Jira bug.

## Scrum Master Bug Responsibilities

As Scrum Master, Idah is responsible for:

- Reviewing new bugs during daily standup
- Confirming each bug has a clear owner
- Ensuring each bug has priority and labels
- Escalating Highest priority bugs to Greg immediately
- Tracking bug progress on the sprint board
- Confirming bugs are resolved before sprint closure
- Closing bugs only after the reporter or owner confirms resolution

## Definition of Done for Bugs

A bug can be closed when:

- The issue has been reproduced or validated
- The fix or resolution has been documented
- The responsible owner confirms completion
- Any related GitHub branch, commit, or PR is linked
- The Jira ticket has the correct final status
- Evidence is attached or referenced where needed
