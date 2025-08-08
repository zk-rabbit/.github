# Contribution

Thank you for your interest in contributing to our projects!

Feel free to dive in. Read the following sections to learn about our workflow and standards. Whether you're looking to write code, contribute to documentation, report bugs, or just ask questions, we appreciate all forms of contribution.

We're really glad you're reading this! Volunteer developers can help us quickly reach our goals and make our projects come to fruition.

## Setup

### .gitmessage

We recommend that every repository provides a `.gitmessage`.
You can make your own `.gitmessage` using [.gitmessage.template](/.gitmessage.template).

Once you create this `.gitmessage`, please add it into your `.git/config` with the following command:

```shell
git config commit.template /path/to/.gitmessage
```

## General Workflow

Follow this workflow when working on our repositories:

1. Select or create an issue.
   - Note: If the "issue" is straightforward, you do not need to create a new issue.
2. Create a new branch for this issue following our [branch guideline](/BRANCH_GUIDELINE.md).
3. On the new branch, make your changes to solve the issue.
   - If you work on the code...
     1. Use the [Google Style Guides](https://google.github.io/styleguide/) to standardize your code.
     2. Test your code against...
        - A formatting tool
        - A lint tool
        - Unittests
4. Commit your changes following our [commit message guideline](/COMMIT_MESSAGE_GUIDELINE.md) below.
5. Open a [pull request](#pull-requests) for all your commits.
6. Request and wait for reviews on your pull request.
7. Fix any problems from comments or reviews received. See [Reviews](#reviews) for more.

The last reviewer will merge and close the PR once an `Approve` review is given by every other reviewer and [the CI](#ci-github-actions) has finished running successfully.

## Issues

The best way to contribute to our projects is by opening a new issue or tackling one of the existing issues.

## Pull Requests

### Before opening a PR

Before opening a pull request for all your commits, we request that you run a final self-check to reduce the amount of potentially trivial errors.
Please ensure these rules are met:

- No typos in the header and body of your commits.
- The changes in each commit do not encompass more than one type of commit. (e.g. A commit that includes `style` and `test` changes should be separated into two different commits)
- The subject of each commit accurately explains the changes made.
- Your PR does not contain any intermediate changes (e.g. An error is made in one commit and rectified in the next commit) among commits.

### Reviews

Reviews should be an interactive experience between the PR author and the reviewers. Unless, the review type is `Approve`, the PR author and the reviewers should acknowledge and work together on the reviews.

Reviews should follow the following process:

1. A reviewer leaves a `Comment` or a `Request Changes` review.
2. The PR author acknowledges the review and/or asks follow-up questions.
3. Once the PR author has all the information they need, they resolve the problem with new changes.
4. The PR author re-requests the reviewer to check their new changes.
5. Based on the reviewer's response, the process starts again or finishes.
   1. Start again - More review is needed and the reviewer submits another `Comment` or `Request Changes` review.
   2. Finish - All new changes are good and reviewer resolves their review.

Note: Comments and reviews may only be resolved by their authors!

Once a reviewer is satisfied with the commits, they will leave an `Approve` review with a comment such as "LGTM."

## Useful Tips

### Before Committing

Before any commits, we recommend to rebase your local repository to prevent any conflicts.

```shell
git fetch origin -p
git rebase origin/main
```

### How to check your changes

Use the following `git` commands to check your changes by category.
You can check your overall status with `git status`.

- Changes not staged for a commit: check with `git diff`.
- Changes to be committed: check with `git diff --cached`.
- Committed changes: check with `git log -p`.

## Other

### CI (Github Actions)

We use GitHub Actions to verify that the code in your PR passes all our checks.

When you submit or update your PR, a CI build will automatically start. A note will be added to the PR that will indicate the current status of the build.

## Questions?

Always feel free to reach out to those actively working on the repositories for any questions you have.
