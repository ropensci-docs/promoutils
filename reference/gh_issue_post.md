# Create a GH issues post

Opens an issue on Github with title, body and labels.

## Usage

``` r
gh_issue_post(
  title,
  body,
  labels,
  owner,
  repo,
  avoid_dups = TRUE,
  dry_run = FALSE,
  open_browser = TRUE
)
```

## Arguments

- title:

  Character. Title of the issue.

- body:

  Character. Body text of the issue.

- labels:

  Character vector. Vector of labels to assign.

- owner:

  Character. GitHub username or organization owner of the repository.

- repo:

  Character. Repository in which to create issue.

- avoid_dups:

  Logical. If TRUE (default), avoids posting duplicate issues.

- dry_run:

  Logical. Whether to do a dry run (i.e. don't post).

- open_browser:

  Logical. Whether to open the issue in the browser.

## Examples

``` r
gh_issue_post(
  title = "My issue",
  body = "Body of the issue",
  labels = "help-wanted",
  owner = "ropensci",
  repo = "weathercan",
  dry_run = TRUE
)
#> 
#> ── Post to  [DRY RUN] ──
#> 
#> title: My issue
#> labels: help-wanted
#> body:
#> Body of the issue
```
