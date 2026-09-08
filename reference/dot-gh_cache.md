# Create a cached version of the GH api calls

Create a cached version of the GH api calls

## Usage

``` r
.gh_cache(..., .token = key("github"), .max_rate = NULL)
```

## Arguments

- ...:

  Arguments passed on to
  [`gh::gh`](https://gh.r-lib.org/reference/gh.html)

  `endpoint`

  :   GitHub API endpoint. Must be one of the following forms:

      - `METHOD path`, e.g. `GET /rate_limit`,

      - `path`, e.g. `/rate_limit`,

      - `METHOD url`, e.g. `GET https://api.github.com/rate_limit`,

      - `url`, e.g. `https://api.github.com/rate_limit`.

      If the method is not supplied, will use `.method`, which defaults
      to `"GET"`.

  `per_page,.per_page`

  :   Number of items to return per page. If omitted, will be
      substituted by `max(.limit, 100)` if `.limit` is set, otherwise
      determined by the API (never greater than 100).

  `.destfile`

  :   Path to write response to disk. If `NULL` (default), response will
      be processed and returned as an object. If path is given, response
      will be written to disk in the form sent. gh writes the response
      to a temporary file, and renames that file to `.destfile` after
      the request was successful. The name of the temporary file is
      created by adding a `-<random>.gh-tmp` suffix to it, where
      `<random>` is an ASCII string with random characters. gh removes
      the temporary file on error.

  `.overwrite`

  :   If `.destfile` is provided, whether to overwrite an existing file.
      Defaults to `FALSE`. If an error happens the original file is
      kept.

  `.api_url`

  :   Github API url (default: <https://api.github.com>). Used if
      `endpoint` just contains a path. Defaults to `GITHUB_API_URL`
      environment variable if set.

  `.method`

  :   HTTP method to use if not explicitly supplied in the `endpoint`.

  `.limit`

  :   Number of records to return. This can be used instead of manual
      pagination. By default it is `NULL`, which means that the defaults
      of the GitHub API are used. You can set it to a number to request
      more (or less) records, and also to `Inf` to request all records.
      Note, that if you request many records, then multiple GitHub API
      calls are used to get them, and this can take a potentially long
      time.

  `.accept`

  :   The value of the `Accept` HTTP header. Defaults to
      `"application/vnd.github.v3+json"` . If `Accept` is given in
      `.send_headers`, then that will be used. This parameter can be
      used to provide a custom media type, in order to access a preview
      feature of the API.

  `.send_headers`

  :   Named character vector of header field values (except
      `Authorization`, which is handled via `.token`). This can be used
      to override or augment the default `User-Agent` header:
      `"https://github.com/r-lib/gh"`.

  `.progress`

  :   Whether to show a progress indicator for calls that need more than
      one HTTP request.

  `.params`

  :   Additional list of parameters to append to `...`. It is easier to
      use this than `...` if you have your parameters in a list already.

  `.max_wait`

  :   Maximum number of seconds to wait if rate limited. Defaults to 10
      minutes.

- .token:

  Authentication token. Defaults to
  [`gh_token()`](https://gh.r-lib.org/reference/gh_token.html).

- .max_rate:

  Maximum request rate in requests per second. Set this to automatically
  throttle requests.

## Details

`memoise::memoise(gh::gh)`
