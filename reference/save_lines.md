# Save text (a container of strings) to a file

Save text (a container of strings) to a file

## Usage

``` r
save_lines(filename, lines)
```

## Arguments

- filename:

  filename of the file to have the text written to

- lines:

  lines of text to be written to file

## Value

Nothing. Will save the lines to file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
text <- c("hello", "world")
filename <- get_beastier_tempfilename()
save_lines(filename = filename, lines = text)
file.remove(filename)
#> [1] TRUE

remove_beaustier_folders()
```
