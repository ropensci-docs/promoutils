# Create url from content date and slug

Create url from content date and slug

## Usage

``` r
url_from_path(
  path,
  date = NULL,
  lang = NULL,
  where = "blog",
  base_url = "https://ropensci.org"
)
```

## Arguments

- path:

  Character. Slug, URL, or path to file in repository

- date:

  Character. Date for event, used to create link (otherwise extracted
  from slug)

- lang:

  Character. Language of blogpost (i.e., `en`, `es`, `fr`, etc.)

- where:

  Character. 'blog' or 'event' depending on the content type.

- base_url:

  Character. Base url of blog posts.

## Value

Full url

## Examples

``` r
url_from_path("my-post", date = "2025-01-01")
#> https://ropensci.org/blog/2025/01/01/my-post/
url_from_path("2025-01-01-my-post/index.es.md")
#> https://ropensci.org/es/blog/2025/01/01/my-post/
url_from_path("content/blog/2025-09-29-news-september-2025/index.md")
#> https://ropensci.org/blog/2025/09/29/news-september-2025/
url_from_path("content/blog/2025-09-29-news-september-2025/index.Rmd")
#> https://ropensci.org/blog/2025/09/29/news-september-2025/
url_from_path("content/blog/2025-09-29-news-september-2025/")
#> https://ropensci.org/blog/2025/09/29/news-september-2025/
```
