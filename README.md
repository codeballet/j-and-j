# j-and-j
## Introduction
The 'j-and-j' repo is an open-ended, collaborative experiment by John Rajeski and Johan Stjernholm.
## Git style guide
### Use of Branches
There are three main branches:
- master
- stage
- dev

The master and stage branches are protected and any pull request needs to be reviewed and approved.

The dev branch is open and used for development. However, please do not make changes straight into the dev branch. Instead, use sub-branches that merge with the dev branch once the topic of the sub-branch is finished.

#### Using sub-branches
Please use sub-branches off the dev branch for making code changes. Sub-branches do not have to be pushed to the repo, but can reside on the local computer.

When naming sub-branches, please use the first letter of the 'type' of the commit, as explained below, followed by a short description of the purpose or the affected file of the branch.

Examples:
| sub-branch | commit                            |
| ---------  | --------------------------------- |
| `f-index`  | `feat: add title`                 |
| `f-auth`   | `fix: change auth connection url` |
| `d-readme` | `docs: add git commit policy`     |

### Commit Messages
When writing git commit messages, please adhere to the style recommended by [Udacity](https://udacity.github.io/git-styleguide/). Below is an extract of the recommendations for the 'Type' and the 'Subject'.

#### The Type
The type is contained within the title and can be one of these types:
- feat: a new feature
- fix: a bug fix
- docs: changes to documentation
- style: formatting, missing semi colons, etc; no code change
- refactor: refactoring production code
- test: adding tests, refactoring test; no production code change
- chore: updating build tasks, package manager configs, etc; no production code change

#### The Subject
Subjects should be no greater than 50 characters, should begin with a capital letter and do not end with a period.

Use an imperative tone to describe what a commit does, rather than what it did. For example, use 'change'; not 'changed' or 'changes'.