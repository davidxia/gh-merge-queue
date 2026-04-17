# gh-merge-queue

A [GitHub CLI](https://cli.github.com) extension for viewing the merge queue of a repository.

## Installation

```sh
$ gh extension install davidxia/gh-merge-queue

$ gh extension list
NAME            REPO                     VERSION 
gh merge-queue  davidxia/gh-merge-queue  d118d76d

$ gh alias set mq merge-queue
```

## Usage

```sh
# Auto-detect repo from current directory
$ gh merge-queue

# Explicit org/repo
$ gh merge-queue modal-labs/modal
2. #1 [AWAITING_CHECKS] make Modal reliable
   by @davidxia • enqueued 28m ago • est. merge in 23m
3. #2 [MERGEABLE] Make Modal fast
   by @AmitPr • enqueued 24m ago • est. merge in 27m
1. #3 [AWAITING_CHECKS] Make Modal powerful
   by @mwaskom • enqueued 35m ago • est. merge in 20m
```

## References

- [gh extension docs](https://cli.github.com/manual/gh_extension)
- [Creating GitHub CLI extensions](https://docs.github.com/en/github-cli/github-cli/creating-github-cli-extensions)
