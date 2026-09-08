# Common arguments and documentation for various functions

Common arguments and documentation for various functions

## Arguments

- test_run:

  Logical. Whether to do a test run (i.e. post to a test area).

- dry_run:

  Logical. Whether to do a dry run (i.e. don't post).

- open_browser:

  Logical. Whether to open the issue in the browser.

- quiet:

  Logical. Whether to suppress progress messages.

- verbose:

  Logical. Show extra informative messages.

- print:

  Logical. Whether to simply print the text to console instead of
  copying to the clipboard.

- force_masto:

  Logical. Passed to
  [`monarch::add_handles()`](https://rdrr.io/pkg/monarch/man/add_handles.html).
  Whether or not to force a re-check of mastodon handles (good if you
  think they've changed or they are 'none' and you want to check again).

## Details

Use `@inheritParams common_docs` to include the above in any function
documentation with a matching argument (will only include matching args)
