# SE-Git-hw

Daniel Ogbuigwe | CINS 5318 - Software Engineering | Fall 2026

This assignment demonstrates Git commits, branches, pull requests, merge conflicts, and GitHub Issues.

## Files

- `helloworld.cpp`: prints `Hello, World!`.
- `apple.py`: feature; prints `I eat apple`.
- `apple.cpp`: additional C++ version of the feature.
- `conflict-demo.txt`: resolved merge-conflict example.

## Run

Requires Python 3 and a C++ compiler.

```bash
python3 apple.py
c++ helloworld.cpp -o /tmp/se-git-hello
/tmp/se-git-hello
c++ apple.cpp -o /tmp/se-git-apple
/tmp/se-git-apple
```

All three programs produced the expected output during local verification.

## Branches and pull request

The initial commit added the README and Hello, World! program. On `feature-1`, I added the apple programs and fixed C++ namespace usage.

[PR #1](https://github.com/ogbidaniel/SE-Git-hw/pull/1) was approved by `ashiqur02` and merged into `main`.

## Merge conflict and resolution

Both `main` and `conflict-demo` independently added `conflict-demo.txt` with different text:

- `main`: `I eat red apples`
- `conflict-demo`: `I eat green apple`

Running `git merge conflict-demo` caused an add/add conflict. I removed the conflict markers and combined the text:

```text
I eat red and green apples
```

I staged the file, committed the resolution, and pushed both branches. [Commit 62a62a8](https://github.com/ogbidaniel/SE-Git-hw/commit/62a62a8) records the completed merge.

## Issues

- [#2: Update Readme](https://github.com/ogbidaniel/SE-Git-hw/issues/2), assigned to `ogbidaniel`: documentation prepared; close after publishing.
- [#3: Review Repo](https://github.com/ogbidaniel/SE-Git-hw/issues/3), assigned to `ashiqur02`: awaiting review results.

Both issues were open and resolved on September 17, 2026.
