Based on https://github.com/github-actions-up-and-running/pr-comment

# PR Comment Action

This action comments a message on PR.

## Inputs

### `repo-token`

**Required** The GitHub Token for comment on PR.

### `message`

The message to comment on PR.

### `file`

Read comment message from file

## Outputs

### `commentUrl`

The PR comment URL.

## Example Usage

```yaml
uses: fxtr/ga-pr-comment@master
with:
  repo-token: ${{ secrets.GITHUB_TOKEN }}
  message: Nice PR!👍
```

```yaml
uses: fxtr/ga-pr-comment@master
with:
  repo-token: ${{ secrets.GITHUB_TOKEN }}
  file: ./comment.txt
```
