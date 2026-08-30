# Internal function

Check that a file can be created at a certain path.

## Usage

``` r
check_can_create_file(filename, overwrite = TRUE)
```

## Arguments

- filename:

  file that may or may not be created

- overwrite:

  if TRUE, if `filename` already exists, it will be deleted by this
  function

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if a file cannot
be created at a certain path.

## Details

Will [stop](https://rdrr.io/r/base/stop.html) if not. Will
[stop](https://rdrr.io/r/base/stop.html) if the file already exists.
Does so by creating an empty file at the path, and then deleting it.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_can_create_file("my_local_file.txt")
```
