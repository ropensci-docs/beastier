# Check there are no files in the default [beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md) folder

Check there are no files in the default
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
folder. The goal is to make sure no temporary files are left undeleted.
Will [stop](https://rdrr.io/r/base/stop.html) if there are files in the
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
folder

## Usage

``` r
check_empty_beastier_folder(beastier_folder = beastier::get_beastier_folder())
```

## Arguments

- beastier_folder:

  the path to the
  [beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
  temporary files folder

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if there are
files in the
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
folder

## Author

Richèl J.C. Bilderbeek
