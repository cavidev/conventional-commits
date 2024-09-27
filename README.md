# Conventional Commits

```text
                                     88           88
                                     ""           88
                                                  88
 ,adPPYba,  ,adPPYYba,  8b       d8  88   ,adPPYb,88   ,adPPYba,  8b       d8
a8"     ""  ""     `Y8  `8b     d8'  88  a8"    `Y88  a8P_____88  `8b     d8'
8b          ,adPPPPP88   `8b   d8'   88  8b       88  8PP"""""""   `8b   d8'
"8a,   ,aa  88,    ,88    `8b,d8'    88  "8a,   ,d88  "8b,   ,aa    `8b,d8'
 `"Ybbd8"'  `"8bbdP"Y8      "8"      88   `"8bbdP"Y8   `"Ybbd8"'      "8"
```

The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This convention dovetails with SemVer, by describing the features, fixes, and breaking changes made in commit messages.

```bash
<type>(<optional scope>): <header description>
empty separator line
<optional body>
empty separator line
<optional footer>
```

### Types Commits

- feat: This commit is to add a new feature
- fix: This commit is to fix a bug
- refactor: This commit is to re-write/re-structure your code, however does not change any API behaviour
- - perf: this is by special refactor commit, that improve performance
- style: This don't affect the meaning (white-space, formatting, missing semi-colons, etc)
- test: This commit is to add missing tests or correcting existing tests
- docs: This commit affects documentation only
- build: This commit affects build components like build tool, ci pipeline, dependencies, project version, etc
- ops: This commit affects operational components like infrastructure, deployment, backup, recovery, etc
- chore: This is a miscellaneous commits e.g. modifying .gitignore or config files.

### Optional Scope

- UI | Backend | Database | `<ticket number>`

#### Semantic Versioning

```md
<version core> ::= <major> "." <minor> "." <patch>
```

## My personal convention ([with emojis](https://gitmoji.dev/)) 👨🏽‍💻

Note: In my opinion, to use conventional commit standards can enhance code readability and maintainability because you can track each commit

commands:

- git add .
- git commit (this will open the file commit editor)

### Init project or new branch

```md
init(<optional scope>): :tada: <header>

<message>
```

### Commiting User Story

These commits are releating with the <minor> version

```md
feat(<optional scope>): :sparkles: <header>

<message>
```

### Commiting Fix Bug

These commits are releating with the <patch> version

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
refactor(<optional scope>): :rotating_light: <header>

<message>
```

```md
chore(<optional scope>): :heavy_minus_sign: <header>

<message>
```

References:

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [git-conventional-commits](https://platform.uno/docs/articles/uno-development/git-conventional-commits.html)
