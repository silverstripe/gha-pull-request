# GitHub Actions - Pull request

Create a new branch, makes a commit and a creates a pull-request using with a github-actions user as the author. These will be created on the account/repo that called the actions.

This action is intended as a step in a larger workflow and at a minimum the repository must have already been checked out and be on the branch that we want to target and there must be some changes to commit.

## Usage

**workflow.yml**
```yml
steps:
  - name: Create pull-request
    uses: silverstripe/gha-pull-request@v1
    with:
      branch: pulls/4/my-branch
      title: NEW My pull-request title
      description: (Optional) This text will appear in the body of the GitHub pull-request
```
