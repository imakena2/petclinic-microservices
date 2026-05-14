# GPM-138: Jira Status Movement for GitHub Work

## Purpose

This document explains how Jira ticket statuses should move when GitHub work is created, reviewed, and completed.

The goal is to make Jira reflect the real progress of GitHub branches, commits, and pull requests.

## Status Flow

To Do -> In Progress -> In Review -> Done

## What Triggers Each Status

| GitHub Action | Jira Status Moves To |
|--------------|----------------------|
| Branch created with GPM ticket number | In Progress |
| Commit pushed with GPM ticket number | In Progress |
| Pull request opened with GPM ticket number | In Review |
| Pull request approved | Testing |
| Pull request merged to dev | Done |

## Manual Status Updates

If automation does not move the ticket automatically, update the Jira ticket manually.

Steps:

1. Open the Jira ticket.
2. Click the current status.
3. Select the correct new status.
4. Add a short comment explaining the update.
5. Save the change.

## Jira Board Columns

| Jira Column | Meaning |
|------------|---------|
| To Do | Work has not started |
| In Progress | A branch or commit exists |
| In Review | A pull request has been opened |
| Testing | Work is being validated |
| Done | Pull request has been merged and accepted |

## Scrum Master Responsibilities

As Scrum Master, Idah should:

- Review ticket statuses daily
- Confirm that active GitHub branches are reflected in Jira
- Confirm that open pull requests are reflected in Jira
- Follow up on tickets stuck in In Progress
- Escalate blocked tickets to Greg
- Confirm completed work before moving tickets to Done

## Definition of Done

GPM-138 can be moved to Done when:

- Jira status flow is documented
- GitHub actions and Jira status movements are mapped
- Manual update steps are documented
- Scrum Master responsibilities are documented
- This document is committed and pushed to GitHub
