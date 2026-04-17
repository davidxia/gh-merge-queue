# gh-merge-queue

A [GitHub CLI](https://cli.github.com) extension for viewing the merge queue of a repository.

## Installation

### Dependencies

* [jq]

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
1. #34 [AWAITING_CHECKS] make Modal reliable
   by @davidxia • enqueued 28m ago • est. merge in 20m
2. #35 [MERGEABLE] Make Modal fast
   by @AmitPr • enqueued 24m ago • est. merge in 23m
3. #39 [AWAITING_CHECKS] Make Modal powerful
   by @mwaskom • enqueued 15m ago • est. merge in 27m
```

## References

- [gh extension docs](https://cli.github.com/manual/gh_extension)
- [Creating GitHub CLI extensions](https://docs.github.com/en/github-cli/github-cli/creating-github-cli-extensions)

[jq]: https://jqlang.org/download/
