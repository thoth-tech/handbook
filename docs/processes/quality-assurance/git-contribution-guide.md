# Git Contribution Guide

[Contributing to Repositories: How To](#contributing-to-repositories-how-to)

[Branching Guidelines](#branching-guidelines)

[Commit Guidelines](#commit-guidelines)

- [Message format](#message-format)

[Code Review Guidelines](#code-review-guidelines)

[Git Workflow Summary](#git-workflow-summary)

## Contributing to Repositories: How To

Repositories are where existing Thoth Tech code is stored, and where new code contributions, once
tested and approved, will ultimately be merged.

In order to begin new work on your project, you will need to clone a local copy of the relevant
Thoth Tech repository.

Steps:

_If you have never worked on the repository before:_

- Clone your project's relevant Thoth Tech repository to your local machine and navigate to the
  created project folder; you will find yourself on the default branch (main/master).

_If you already have a copy of this repository on your local machine_

- From the main/master branch of your local copy of the repository, make sure to do a git "pull" to
  make sure you are working on the latest copy of code from the origin (this will include any
  changes merged to the main branch since you last cloned/pulled the repo).

_Then:_

- Create a new branch (as per [Branching Guide](#branching-guidelines)) for your changes
- Make your code changes on the branch you created
- When complete, commit your changes, using the format provided in the
  [commit guidelines](#commit-guidelines).
- Push the branch to origin
- Create a [draft Pull Request](#draft-pull-request) (PR) for merging the branch into the main Thoth
  Tech branch for your repository, adding [required approvals](#required-approvals) (note: it will
  be blocked from merging while in draft form). Comment on the progress and any feedback sought.
- Continue making changes on your local branch, committing and pushing your changes, until you are
  satisfied the code is complete, passing all tests and relevant acceptance criteria, and ready for
  merging
- Publish your Pull request by changing the status to ready for review

An example sequence of git commands used in this process is provided in the
[Git Workflow Summary](#git-workflow-summary).

## Branching Guidelines

No commits should be made directly to the default branch (usually main/master/develop). Instead,
branches should be created off the default branch to encompass any changes.

Branches must have descriptive names, including a reference the task/subtask number the work relates
to, using the following format:

| Branch naming format                                   | Use                                            |
| ------------------------------------------------------ | ---------------------------------------------- |
| `feature/<project_task or subtask number_description>` | New product feature/function                   |
| `fix/<project_task or subtask number_description>`     | For a fix                                      |
| `doc/<project_task or subtask number_description>`     | Non-feature-related document additions/changes |

For an example, let's assume the following hypothetical task breakdown for the Voice Verification
project (we might expect these numbers to be reflected in a Trello task cards):

Product/Epic:

_Voice Verification_

_Tasks:_

1. _Voice Registration_

   1.1. _Receive Voice Input_

   1.2. _Store Voice Input_

2. _Voice Matching_
3. _\<task\>_

   3.1 _\<subtask\>_

A programmer who is going to commence work on the Voice Verification component subtask 1.2 should
use a branch named: _feature/voice-verification-1.2-store-voice-input_

This would be created and checked out by using the git command:

```shell
git checkout -b feature/voice-verification-1.2-store-voice-input
```

## Commit Guidelines

Thoth Tech follows the same Git commit message format as required by the Doubtfire LMS (source
doubtfire-lms's
[CONTRIBUTING.md](https://github.com/doubtfire-lms/doubtfire-deploy/blob/development/CONTRIBUTING.md#commit-message-format))
which this section predominantly mirrors. This format makes for an easier to read and more useful
commit history.

### Message Format

Each commit message consists of a header, a body, and a footer.

```plaintext
<header>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory and must conform to the Commit Message Header format.

The **body** is recommended for all commits. When the body is present, it must be at least 20
characters long and conform to the Commit Message Body format.

The **footer** is optional. The Commit Message Footer format describes the purpose and structure of
the footer.

Any line of the commit message should be 100 characters or fewer.

```plaintext
Commit Message Header
<type>(<scope>): <short summary>
  │       │             │
  │       │             └─⫸ Summary in present tense. Not capitalized. No period at the end.
  │       │
  │       └─⫸ Commit Scope (optional): animations|common|style|forms|http|router|service-worker|
  │                                     upgrade|changelog|dev-infra|docs-infra|migrations|
  │
  └─⫸ Commit Type: build|ci|docs|feat|fix|perf|refactor|test
```

The `<type>` and `<summary>` fields are mandatory, the (`<scope>`) field is optional.

The `<type>` must be one of the following:

- **build** : Changes that affect the build system or external dependencies (example scopes: gulp,
  broccoli, npm)
- **ci** : Changes to our CI configuration files and scripts (example scopes: Circle, BrowserStack,
  SauceLabs)
- **docs** : Documentation only changes
- **feat** : A new feature
- **fix** : A bug fix
- **perf** : A code change that improves performance
- **refactor** : A code change that neither fixes a bug nor adds a feature
- **test** : Adding missing tests or correcting existing tests

Doubtfire-LMS recommends Chris Beam's post on
[How to Write Good Commit Messages](http://chris.beams.io/posts/git-commit/) to improve your commit
message writing.

**Use the imperative mood in your commit subject line**

Write your commits in the imperative mood and not the indicative mood

- "Fix a bug" and **not** "Fix*ed* a bug"
- "Change the behaviour of Y" and **not** "_Changed_ the behaviour of Y"
- "Add new API methods" and **not** "Sweet new API methods"

Keep the subject line (top line) concise; keep it **within 50 characters**.

Use the body (lines after the top line) to explain why and what and _not_ how; keep it **within 72
characters**.

### But how can I write new lines if I'm using `git commit -m "Message"`?

Don't use the `-m` switch. Use a text editor to write your commit message instead.

If you are using the command line to write your commits, it is useful to set your git editor to make
writing a commit body easier. You can use the following command to set your editor to Visual Studio
Code, `nano`, `emacs`, `vim`, `atom`.

```shell
git config --global core.editor "code --wait"
git config --global core.editor nano
git config --global core.editor emacs
git config --global core.editor vim
git config --global core.editor "atom --wait"
```

## Code Review Guidelines

You are strongly encouraged to get your code reviewed by a reviewer as soon as there is any code to
review, to get a second opinion on the chosen solution and implementation, and an extra pair of eyes
looking for bugs, logic problems, or uncovered edge cases.

### Draft Pull Request

Draft Pull Requests allow a work in progress to receive early feedback. The developer creating the
PR should, in the description, indicate their progress and any particular aspect they are looking
for feedback on. When the PR is ready for final review, the developer should update the description,
re-request reviews as required and change the status to "ready to review".

Pull requests (draft and otherwise) are created from the GitHub website. Further information about
draft pull requests, how to make them, and how to convert their status to ready for merging can be
found on GitHub's
[Introducing Draft Pull Requests](https://github.blog/2019-02-14-introducing-draft-pull-requests/)
blog.

### Required Approvals

Pull requests require **a minimum of two approvals**. The default approach is to choose a reviewer
from your team for the first review. However, the reviewer may be from different team, for example a
domain expert in a programming language, quality assurance process, telemetry or documentation.
Depending on the team size and dynamics, the number of required approvals can be higher or lower.
Think about the tradeoffs between velocity with quality when deciding on an approval process for
your team.

The required approvals rules can be set via the
[branch protection rule](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/defining-the-mergeability-of-pull-requests/managing-a-branch-protection-rule).
All the leads should have access to change these settings and should ensure this is configured when
creating a new GitHub repository. For more information on how to set this up correctly, see this
[guide](https://github.com/thoth-tech/handbook/blob/main/docs/learning/useful-resources/setup-new-github-repository.md).

## Git Workflow Summary

### Start a new piece of work

1. Synch repo and set up for your new feature branch (remember to use Thoth Tech
   [branching guidelines](#branching-guidelines) for naming the new branch; we have used the
   guideline example of _feature/voice-verification-1.2-store-voice-input_ for our workflow
   illustration):

   ```shell
   git checkout main
   git pull main
   git checkout -b feature/voice-verification-1.2-store-voice-input
   ```

2. Make changes, commit (using comments format that follows [commit guidelines](#commit-guidelines))
   and push to origin:

   ```shell
   git add .
   git commit
   git push -u origin feature/voice-verification-1.2-store-voice-input
   ```

3. Remember to submit a [draft pull request](#draft-pull-request) via GitHub to allow for code
   review (and mark as ready to submit when ready to merge your changes to main).

### Continue a piece of work

1. If the branch has already been created in the remote repository.

   ```shell
   git checkout feature/voice-verification-1.2-store-voice-input
   ```

2. Pull in any new code from the default branch

   ```shell
   git pull origin main
   ```

3. Resolve any merge conflicts that may now be revealed.

4. Continue to Step 2 in [Start a new piece of work](#start-a-new-piece-of-work) flow

### Collaborate on an existing branch

Ideally, we should avoid having developers working on the same code. It creates merge conflicts and
hinders efficiency. If possible, try to break it down into small tasks so developers can work
independently. In the worst-case scenario, if there is more than 1 person working on a feature
branch:

1. Please make sure you pull changes in the remote branch before starting your work.

   ```shell
   git pull origin feature/voice-verification-1.2-store-voice-input
   ```

2. Resolve any merge conflicts that may now be revealed.
3. Continue to Step 2 in [Start a new piece of work](#start-a-new-piece-of-work) flow

**Please avoid force-push and rebase when working on a shared branch**. It can cause complex and
hard to resolve merge conflicts as well as undo others' commits accidentally.
