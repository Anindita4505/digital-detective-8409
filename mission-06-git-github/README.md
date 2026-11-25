# Mission 6 — Git and GitHub

## 1. Task / Objective

The objective of this mission was to understand version control, practise the basic Git workflow, create and publish a branch, open a Pull Request, and learn important Git commands.

## 2. Work Completed

### Task 6.1 — Understand the Basic Git Workflow

Inspected the repository status and recent commit history using Git commands.

| Git operation           | What it does                                         |
| ----------------------- | ---------------------------------------------------- |
| Check repository status | Shows modified, staged, and untracked files.         |
| Stage selected changes  | Selects changes to be included in the next commit.   |
| Create a commit         | Saves staged changes as a checkpoint in Git history. |
| View commit history     | Displays previous commits and their messages.        |

**Difference between staging and committing:**

Staging using `git add` selects the changes that should be included in the next commit. Committing using `git commit` permanently records those staged changes in the repository's history.
Commit hash : 'aecf8f2'

### Task 6.2 — Create and Use a Branch

Created a new branch named `update-about`.

Added a **My Learning** section to the root `README.md`, describing concepts learned during the assignment.

Committed the change with the message:

`Add My Learning section to README`

Commit hash: `59d3cfb`

Published the branch to GitHub using `git push -u origin update-about`.

### Task 6.3 — Create a Pull Request

Created Pull Request #1 on GitHub.

- **Title:** Add My Learning section to README
- **Base branch:** `main`
- **Compare branch:** `update-about`
- **Status:** Open (not merged)

Reviewed the changed file and confirmed that GitHub reported no merge conflicts.

The Pull Request demonstrates how changes can be reviewed before being merged into the main branch.

**Note:** The Pull Request has intentionally not been merged because the assignment instructs merging only if the instructor asks for it.

### Task 6.4 — Git Command Glossary

| Git operation           | Command                                 | Explanation                                            |
| ----------------------- | --------------------------------------- | ------------------------------------------------------ |
| Initialise a repository | `git init`                              | Creates a new Git repository in the current folder.    |
| Check status            | `git status`                            | Shows which files are modified, staged, or untracked.  |
| Stage changes           | `git add filename`                      | Selects a file's changes for the next commit.          |
| Commit changes          | `git commit -m "message"`               | Saves staged changes as a new commit.                  |
| View history            | `git log --oneline`                     | Displays commit history in a compact format.           |
| Create or list branches | `git branch branch-name` / `git branch` | Creates a branch or lists existing local branches.     |
| Switch branches         | `git switch branch-name`                | Switches to another branch.                            |
| Publish changes         | `git push origin branch-name`           | Uploads local commits to the remote repository.        |
| Retrieve remote changes | `git pull origin branch-name`           | Downloads and integrates changes from a remote branch. |

## 3. Commands / Tools Used

| Command or tool                                     | Purpose                                 |
| --------------------------------------------------- | --------------------------------------- |
| `git status`                                        | Checked repository status.              |
| `git log --oneline`                                 | Inspected recent commit history.        |
| `git branch`                                        | Listed local branches.                  |
| `git switch -c update-about`                        | Created and switched to the new branch. |
| `git diff README.md`                                | Reviewed changes to the root README.    |
| `git add README.md`                                 | Staged the README change.               |
| `git commit -m "Add My Learning section to README"` | Committed the branch change.            |
| `git push -u origin update-about`                   | Published the branch to GitHub.         |
| GitHub Pull Requests                                | Created and reviewed Pull Request #1.   |

## 4. My Understanding

Git is a version control system that tracks changes in files and maintains a history of those changes. GitHub is an online platform that hosts Git repositories and supports collaboration.

A branch is a separate line of development that allows changes to be made without directly modifying the main branch.

A Pull Request is a request to review and merge changes from one branch into another. It helps team members discuss and review changes before they become part of the main project.

Branches and Pull Requests make collaboration safer and help keep the main project organised.

Working with branches and Pull Requests also taught me how developers can review changes separately before integrating them into the main project.

## 5. Difficulties Faced

No major technical difficulties were faced during this mission.

## 6. How I Resolved Them

Followed the Git workflow step by step, checked repository status and differences before committing, and verified the branch and Pull Request on GitHub.

## 7. Evidence / Files

- Root `README.md` containing the new My Learning section.
- This Mission 6 README containing the Git explanations and glossary.
- GitHub branch: `update-about`.
- GitHub Pull Request: #1 — Add My Learning section to README.
- Pull Request status: Open and not merged.
- `evidence/mission-06-git-workflow.png` — Git workflow evidence.
- `evidence/mission-06-pull-request.png` — Pull Request evidence.

## 8. Commit Details

**Task 6.1 commit:**

- Branch: `main`
- Commit hash: `aecf8f2`
- Message: `Document Git workflow basics`

**Task 6.2 commit:**

- Branch: `update-about`
- Commit hash: `59d3cfb`
- Message: `Add My Learning section to README`

**Final Mission 6 documentation commit:**

- Branch: `main`
- Commit message: `Complete Git and GitHub collaboration mission`
- Includes this README and the two Mission 6 evidence screenshots.
