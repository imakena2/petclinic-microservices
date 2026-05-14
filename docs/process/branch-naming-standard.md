# GPM-132: Jira-Linked Branch Naming Standard

## Purpose

This document defines the official branch naming standard for the Achievers11-DevOps PetClinic project.

The goal is to make sure every GitHub branch is linked clearly to the correct Jira ticket.

## Official Branch Naming Convention

All feature branches must follow this format:

feature/GPM-{ticket-number}-{your-name}-{short-description}

## Branch Naming Rules

- Always start with: feature/
- Always include the Jira ticket number: GPM-{number}
- Always include your name in lowercase
- Always use a short description at the end
- Use hyphens instead of spaces
- Create branches from main
- Do not create a new feature branch from another feature branch

## Correct Examples

| Ticket | Branch Name |
|--------|-------------|
| GPM-132 | feature/GPM-132-idah-branch-naming-standard |
| GPM-139 | feature/GPM-139-idah-jira-github-linking |
| GPM-140 | feature/GPM-140-idah-jira-github-integration |
| GPM-193 | feature/GPM-193-idah-qa-and-bugs |

## Incorrect Examples

| Wrong Branch Name | Reason |
|-------------------|--------|
| gpm-132-idah | Does not start with feature/ |
| feature/132-idah | Missing GPM ticket format |
| feature/GPM 132 idah | Contains spaces |
| feature/idah-branch-standard | Missing Jira ticket number |

## Why This Standard Matters

Jira can automatically detect GitHub work when the branch name includes the Jira ticket number.

For example, when a branch is named:

feature/GPM-132-idah-branch-naming-standard

Jira can link that branch to ticket GPM-132.

This helps the team see:

- Who is working on the task
- Which branch belongs to which ticket
- Whether development work has started
- Whether commits and pull requests are linked

## Commit Message Standard

Every commit should also include the Jira ticket number.

Format:

GPM-{number}: short description of the change

Example:

GPM-132: add Jira-linked branch naming standard

## Pull Request Title Standard

Every pull request title should include the Jira ticket number.

Example:

GPM-132: define Jira-linked branch naming standard

## Definition of Done

GPM-132 can be moved to Done when:

- The branch naming format is documented
- Correct and incorrect examples are included
- Jira linking purpose is explained
- Commit message standard is documented
- Pull request title standard is documented
- This document is committed and pushed to GitHub
