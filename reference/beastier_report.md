# Creates a [beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md) report

Creates a
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
report, to be used when reporting bugs. Uses
[message](https://rdrr.io/r/base/message.html)

## Usage

``` r
beastier_report(
  beast2_folder = beastier::get_default_beast2_folder(),
  os = rappdirs::app_dir()$os
)
```

## Arguments

- beast2_folder:

  the folder where the BEAST2 is installed. Note that this is not the
  folder where the BEAST2 executable is installed: the BEAST2 executable
  is in a subfolder. Use
  [get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
  to get the default BEAST2 folder. Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the full path to the default BEAST2 executable.

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

No return value, the information will be shown using
[message](https://rdrr.io/r/base/message.html)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

beastier_report()
#> ***********
#> * beastier *
#> ***********
#> OS: unix
#> beast2_folder: ~/.local/share
#> beast2_path: /github/home/.local/share/beast/lib/launcher.jar
#> ****************
#> * Dependencies *
#> ****************
#> beautier version: 2.6.16
#> beastier version: 2.5.3
#> **********
#> * BEAST2 *
#> **********
#> Java version: 21.0.12+8-1-24.04-Ubuntu
#> Is BEAST2 installed: FALSE
#> ****************
#> * session info *
#> ****************
#> ─ Session info ───────────────────────────────────────────────────────────────
#>  setting  value
#>  version  R version 4.6.0 (2026-04-24)
#>  os       Ubuntu 24.04.4 LTS
#>  system   x86_64, linux-gnu
#>  ui       X11
#>  language en-US
#>  collate  C
#>  ctype    en_US.UTF-8
#>  tz       Etc/UTC
#>  date     2026-08-30
#>  pandoc   3.8.3 @ /usr/local/bin/ (via rmarkdown)
#>  quarto   1.9.37 @ /usr/local/bin/quarto
#> 
#> ─ Packages ───────────────────────────────────────────────────────────────────
#>  package     * version date (UTC) lib source
#>  askpass       1.2.1   2024-10-04 [1] RSPM
#>  beastier    * 2.5.3   2026-08-30 [1] local
#>  beautier      2.6.16  2025-12-08 [1] https://r~
#>  bslib         0.12.0  2026-08-04 [1] RSPM
#>  cachem        1.1.0   2024-05-16 [1] RSPM
#>  cli           3.6.6   2026-04-09 [1] RSPM
#>  curl          8.0.0   2026-08-25 [1] RSPM
#>  desc          1.4.3   2023-12-10 [1] RSPM
#>  digest        0.6.39  2025-11-19 [1] RSPM
#>  downlit       0.4.5   2025-11-14 [1] RSPM
#>  evaluate      1.0.5   2025-08-27 [1] RSPM
#>  fansi         1.0.7   2025-11-19 [1] RSPM
#>  fastmap       1.2.0   2024-05-15 [1] RSPM
#>  fontawesome   0.5.3   2024-11-16 [1] RSPM
#>  fs            2.1.0   2026-04-18 [1] RSPM
#>  glue          1.8.1   2026-04-17 [1] RSPM
#>  htmltools     0.5.9   2025-12-04 [1] RSPM
#>  httr2         1.3.0   2026-07-13 [1] RSPM
#>  jquerylib     0.1.4   2021-04-26 [1] RSPM
#>  jsonlite      2.0.0   2025-03-27 [1] RSPM
#>  knitr         1.51    2025-12-20 [1] RSPM
#>  lifecycle     1.0.5   2026-01-08 [1] RSPM
#>  magrittr      2.0.5   2026-04-04 [1] RSPM
#>  memoise       2.0.1   2021-11-26 [1] RSPM
#>  openssl       2.4.2   2026-06-09 [1] RSPM
#>  otel          0.2.0   2025-08-29 [1] RSPM
#>  pillar        1.11.1  2025-09-17 [1] RSPM
#>  pkgconfig     2.0.3   2019-09-22 [1] RSPM
#>  pkgdown       2.2.1   2026-07-07 [1] RSPM
#>  purrr         1.2.2   2026-04-10 [1] RSPM
#>  R6            2.6.1   2025-02-15 [1] RSPM
#>  ragg          1.5.2   2026-03-23 [1] RSPM
#>  rappdirs      0.3.4   2026-01-17 [1] RSPM
#>  remotes       2.5.0   2024-03-17 [2] RSPM (R 4.6.0)
#>  rJava         1.0-18  2026-04-08 [1] RSPM
#>  rlang         1.3.0   2026-07-05 [1] RSPM
#>  rmarkdown     2.31    2026-03-26 [1] RSPM
#>  rotemplate    2.0.1   2026-08-30 [1] Github (ropensci-org/rotemplate@4c36a4f)
#>  rstudioapi    0.19.0  2026-06-11 [1] RSPM
#>  sass          0.4.10  2025-04-11 [1] RSPM
#>  sessioninfo   1.2.4   2026-06-04 [1] RSPM
#>  stringi       1.8.9   2026-08-04 [1] RSPM
#>  stringr       1.6.0   2025-11-04 [1] RSPM
#>  systemfonts   1.3.2   2026-03-05 [1] RSPM
#>  textshaping   1.0.5   2026-03-06 [1] RSPM
#>  tibble        3.3.1   2026-01-11 [1] RSPM
#>  utf8          1.2.6   2025-06-08 [1] RSPM
#>  vctrs         0.7.3   2026-04-11 [1] RSPM
#>  whisker       0.4.1   2022-12-05 [1] RSPM
#>  withr         3.0.3   2026-06-19 [1] RSPM
#>  xfun          0.60    2026-07-09 [1] RSPM
#>  xml2          1.6.0   2026-06-22 [1] RSPM
#>  yaml          2.3.12  2025-12-10 [1] RSPM
#> 
#>  [1] /github/home/R/x86_64-pc-linux-gnu-library/4.6
#>  [2] /usr/local/lib/R/site-library
#>  [3] /usr/lib/R/site-library
#>  [4] /usr/lib/R/library
#>  * ── Packages attached to the search path.
#> 
#> ──────────────────────────────────────────────────────────────────────────────

check_empty_beaustier_folders()
```
