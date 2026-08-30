# Get the full path of a BEAST2 example file

Will [stop](https://rdrr.io/r/base/stop.html) if the filename is not a
BEAST2 example file

## Usage

``` r
get_beast2_example_filename(
  filename,
  beast2_folder = beastier::get_default_beast2_folder()
)
```

## Arguments

- filename:

  name of the BEAST2 example file. This should exclude the full path;
  this function exists to add that full path

- beast2_folder:

  the folder where the BEAST2 is installed. Note that this is not the
  folder where the BEAST2 executable is installed: the BEAST2 executable
  is in a subfolder. Use
  [get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
  to get the default BEAST2 folder. Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the full path to the default BEAST2 executable.

## Value

the full path of a BEAST2 example file, will
[stop](https://rdrr.io/r/base/stop.html) if the filename is not a BEAST2
example file

## Examples

``` r
if (is_beast2_installed()) {
  get_beast2_example_filename("testJukesCantor.xml")
}
```
