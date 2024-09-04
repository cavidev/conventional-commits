# Conventional Commits

The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This convention dovetails with SemVer, by describing the features, fixes, and breaking changes made in commit messages.

```bash
<type>(<optional scope>): <description>
empty separator line
<optional body>
empty separator line
<optional footer>
```

### Types

- feat Commits: that adds or remove a new feature
- fix Commits: that fixes a bug
- refactor Commits: that rewrite/restructure your code, however does not change any API behaviour
- - perf Commits: are special refactor commits, that improve performance
- style Commits: that do not affect the meaning (white-space, formatting, missing semi-colons, etc)
- test Commits: that add missing tests or correcting existing tests
- docs Commits: that affect documentation only
- build Commits: that affect build components like build tool, ci pipeline, dependencies, project version, ...
- ops Commits: that affect operational components like infrastructure, deployment, backup, recovery, ...
- chore Miscellaneous commits e.g. modifying .gitignore

### Optional Scope

- UI
- Backend
- Database

## My personal convention ([with emojis](https://gitmoji.dev/)) 👨🏽‍💻

Note: In my opinion, to use conventional commit standards can enhance code readability and maintainability.

commands:

- git add .
- git commit (this will open the windows editor)

### Commiting User Story

```md
feat(<optional scope>): :sparkles: <header>
<message>
```

### Commiting Fix Bug

```md
fix(<optional scope>): :bug: <header>
<message>
```

### Commiting README, Changelogs and Docs changes

```md
doc(<optional scope>): :memo: <header>
<message>
```

### Commiting test

```md
test(<optional scope>): :white_check_mark: <header>
<message>
```

### Commiting WIP/Progress/MinorChanges

```md
wip(<optional scope>): :construction: <header>
<message>
```

### Removing libraries/dependecies

```md
refactor: :heavy_minus_sign: <header>
<message>
```

References:

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [git-conventional-commits](https://platform.uno/docs/articles/uno-development/git-conventional-commits.html)
