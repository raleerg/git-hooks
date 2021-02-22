# Git Hooks

## Description

### pre-commit

This pre-commit will validate branch naming against **Git Flow** and **Jira ticket number** validators.

Branch format: `(feature|bugfix|hotfix)/(jira-ticket-number)-(branch-description)`

### commit-msg

Check if the **Jira ticket number** is present at the beggining of the commit message. If it's not, it will grab the number from the branch name and ask for confirmation. After confirmation, it will add the number at the beginning of the commit message and commit everything.

### Install

Move hooks into your projects `.git/hooks` folder.
