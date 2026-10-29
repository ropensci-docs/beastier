# Check there are no files in the default \`beautier\` and \`beastier\` folders

Check there are no files in the default \`beautier\` and \`beastier\`
folders.

## Usage

``` r
check_empty_beaustier_folders(
  beautier_folder = beautier::get_beautier_folder(),
  beastier_folder = beastier::get_beastier_folder()
)
```

## Arguments

- beautier_folder:

  temporary folder used by
  [beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html)

- beastier_folder:

  the path to the
  [beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
  temporary files folder

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if there are
files in the
[beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html)
of
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
folder.

## Details

The goal is to make sure no temporary files are left undeleted. Will
[stop](https://rdrr.io/r/base/stop.html) if there are files in the
[beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html)
of
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
folder.

## Author

Richèl J.C. Bilderbeek
