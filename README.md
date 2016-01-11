# Git Guidelines

We use [git](https://git-scm.com/) as our version control system. These guidelines describe how we work with git.

## Our workflow

In [this excellent tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows) by Atlassian some frequently
used workflows are described and compared.

Our workflow is very similar to the [Gitflow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow).
The differences are outlined below.

### Branch names

Our historical branches have other names:

- **master** is called **stable*
- **release** is called **testing**
- **development** is called **master**

### Feature branches

We encourage the use of feature branches, but don't have strict rules about them. That allows teams to design their own
branching strategy, tailored to their needs.

In practice all teams use some form of feature branches, but sometimes changes are committed to a historical branch
without a feature branch.

## Commits

### Small, atomic commits

A commit should be small and represent one logical change. This makes it easy to review the commit and (sometimes)
cherry-pick and revert the change.

A commit should not leave a branch in an inconsistant state. This makes bisect and revert harder.

You should split off non-functional changes (refactoring, boy scouting) to separate commits.

### Commit messages

We spend way more time reading code than writing code. Part of reading code is understanding the history: how and why
did this code become what it is?

Commit messages can help if they're good. Read [this excellent article on good commit messages](http://chris.beams.io/posts/git-commit/).