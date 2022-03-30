# QA Processes

Repositories
Branching Guidelines[TBC]

Branch naming format[TBC]

Draft Pull Request[TBC]

Required Approvals[TBC]

Commit Guidelines[TBC]

Message format[TBC]

Git Workflow Summary[TBC]

## Repositories

Thoth Tech projects use the below repositories:

T1 2022 [project TBC] --> handbook

T1 2022 [project TBC] --> skm

T1 2022 [project TBC] --> arcade-machine Public

T1 2022 [project TBC] --> doubtfire-api

T1 2022 [project TBC] --> git-workshop

T1 2022 [project TBC] --> doubtfire-web

T1 2022 [project TBC] --> dreambig-documentation

T1 2022 [project TBC] --> splashkit-core

T1 2022 [project TBC] --> programming-arcana

T1 2022 [project TBC] --> entity-socket-demo

T1 2022 [project TBC] --> doubtfire-deploy

T1 2022 [project TBC] --> splashkit-translator

T1 2022 [project TBC] --> splashkit.io

T1 2022 [project TBC] --> doubtfire-speaker-verification

Repositories are where existing Thoth Tech code is stored, and where new code contributions, once tested and approved, will ultimately be merged.

In order to begin new work on your project, you will need to clone a local copy of the relevant Thoth Tech repository.

**Steps:**

_If you have never worked on the repository before:_

- Clone your project’s relevant Thoth Tech repository to your local machine and navigate to the created project folder; you will find yourself on the default branch (usually one of main/master/develop).

_If you already have a copy of this repository on your local machine_

- From the default branch of your local copy of the repository, make sure to do a git “pull” to make sure you are working on the latest copy of code from the origin (this will include any changes merged to the main branch since you last cloned/pulled the repo).

_Then:_

- Create a new branch (as per Branching Guide[TBC]) for your changes

- Make your code changes on the branch you created

- When complete, commit your changes, using the format provided in the commit guidelines[TBC]

- Push the branch to origin

- Create a draft Pull Request[TBC] (PR) for merging the branch into the main Thoth Tech branch for your repository, adding required approvals[TBC] (note: it will be blocked from merging while in draft form). Comment on the progress and any feedback sought.

- Continue making changes on your local branch, committing and pushing your changes, until you are satisfied the code is complete, passing all tests and relevant acceptance criteria, and ready for merging.

- Publish your Pull request by changing the status to ready for review.

An example sequence of git commands used in this process is provided in the Git Workflow Summary[TBC].
