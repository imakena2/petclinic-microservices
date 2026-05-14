# GPM-139: Linking Jira Work Items to GitHub Branches, Commits, and Pull Requests

## Purpose

This document explains how Jira work items are linked to GitHub branches, commits, and pull requests in the Achievers11-DevOps PetClinic project.

The goal is to make project tracking easier by ensuring every GitHub action is connected to the correct Jira ticket.

## How Jira and GitHub Linking Works

Jira can detect GitHub activity when the Jira ticket number is included in:

- The branch name
- The commit message
- The pull request title
- The pull request description

Example Jira ticket number:

GPM-139

## Branch Linking

When a branch is created with the Jira ticket number, Jira can link the branch to the ticket automatically.

Example:

feature/GPM-139-idah-jira-github-linking

This tells Jira that the branch belongs to ticket GPM-139.

## Commit Linking

Every commit message should include the Jira ticket number.

Example:

GPM-139: add Jira and GitHub linking documentation

This allows Jira to show the commit under the related ticket.

## Pull Request Linking

Every pull request title should include the Jira ticket number.

Example:

GPM-139: link Jira work items to GitHub branches commits and PRs

This allows Jira to show the pull request under the related ticket.

## Pull Request Description

The pull request description should also mention the Jira ticket number and the file changed.

Example:

Jira Ticket: GPM-139

File Added:
docs/process/jira-github-linking.md

Summary:
Added documentation explaining how Jira links to GitHub branches, commits, and pull requests.

## How to Verify Linking in Jira

1. Open the Jira ticket.
2. Look for the Development section.
3. Confirm that the branch appears.
4. Confirm that commits appear.
5. Confirm that the pull request appears.
6. Confirm that build status appears if CI has run.

## Troubleshooting

| Problem | Possible Fix |
|---------|--------------|
| Branch not showing in Jira | Check that the branch name contains the correct GPM ticket number |
| Commit not showing in Jira | Check that the commit message contains the GPM ticket number |
| Pull request not showing in Jira | Check that the PR title contains the GPM ticket number |
| Nothing is showing | Confirm GitHub for Atlassian integration is connected |
| CI status not showing | Confirm GitHub Actions has run on the branch |

## Best Practice

Always use the Jira ticket number consistently.

Use the ticket number in:

- Branch name
- Commit message
- Pull request title
- Pull request description

## Definition of Done

GPM-139 can be moved to Done when:

- Branch linking process is documented
- Commit linking process is documented
- Pull request linking process is documented
- Jira verification steps are documented
- Troubleshooting steps are documented
- This document is committed and pushed to GitHub
