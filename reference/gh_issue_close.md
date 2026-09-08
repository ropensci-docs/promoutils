# Close a GH issue

Closes a GH issue by number, repository and owner.

## Usage

``` r
gh_issue_close(n, owner, repo, dry_run = FALSE)
```

## Arguments

- n:

  Numeric. Issue number to close.

- owner:

  Character. GitHub username or organization owner of the repository.

- repo:

  Character. Repository in which to create issue.

- dry_run:

  Logical. Whether to do a dry run (i.e. don't post).

## Examples

``` r
if (FALSE) { # \dontrun{
  # Closes the first issue in the "myrop" repository of "myhandle" on GitHub
  gh_issue_close(1, "myhandle", "myrepo")
} # }
```
