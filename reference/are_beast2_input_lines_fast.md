# Would these lines of text, when written to a file, result in a valid BEAST2 input file?

Would these lines of text, when written to a file, result in a valid
BEAST2 input file?

## Usage

``` r
are_beast2_input_lines_fast(lines)
```

## Arguments

- lines:

  lines of text

## Value

TRUE if the text is valid, FALSE if not

## See also

Use
[`is_beast2_input_file`](https://docs.ropensci.org/beastier/reference/is_beast2_input_file.md)
to check a file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r

beast2_filename <- get_beastier_path("anthus_2_4.xml")
text <- readLines(beast2_filename)

# TRUE
are_beast2_input_lines_fast(text)
#> [1] TRUE
check_empty_beaustier_folders()
```
