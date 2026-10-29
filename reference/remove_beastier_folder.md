# Check there are no files in the default [beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html) folder

Check there are no files in the default
[beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html)
folder. The goal is to make sure no temporary files are left undeleted.
Will [stop](https://rdrr.io/r/base/stop.html) if there are files in the
[beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html)
folder.

## Usage

``` r
remove_beastier_folder()
```

## Value

Nothing.

## See also

use
[remove_beautier_folder](https://docs.ropensci.org/beautier/reference/remove_beautier_folder.html)
to remove the default \`beautier\` folder

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beastier_folder()

remove_beastier_folder()

check_empty_beastier_folder()
```
