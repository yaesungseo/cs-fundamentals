# Developer Tools and Git
## Core idea
Git is a distributed version control system. It records project history as commits so you can inspect earlier states, develop changes on branches, and combine work. GitHub hosts Git repositories and adds collaboration features such as pull requests and issues.

A repository includes tracked content and its history. A commit records a snapshot and metadata, including links to parent commits. A branch is a movable reference to a commit.

## The three places to understand
- Working tree: the files you are editing.
- Staging area (index): the content selected for the next commit.
- Repository history: the commits already recorded.

Saving a file does not commit it. Committing locally does not upload it to GitHub.

## Example
Inside an existing practice repository, after creating a file named notes.md:
```sh
git status
git diff
git add notes.md
git diff --staged
git commit -m "Add introductory notes"
git log --oneline
```

A remote is a named reference to another repository. Fetch downloads remote history; push sends local commits and updates remote references when permitted. Pull fetches and then integrates changes according to its options and configuration.

## Common confusion
A terminal is an interface for text interaction. A shell interprets commands. Git is one program you can run from a shell. A pull request is a hosting-platform collaboration feature, not a Git commit.

## Try it
Change notes.md after staging it. Compare git diff with git diff --staged. Which version would the next commit contain?

## Expand next
Branches and merges; merge conflicts; .gitignore; pull requests; shell paths and environment variables.

## Reference
[Pro Git: What is Git?](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F)

[Back to index](../../README.md)
