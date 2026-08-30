# Create a temporary filename for the BEAST2 XML filename

Create a temporary filename for the BEAST2 XML filename

## Usage

``` r
create_temp_input_filename()
```

## Value

a temporary filename, that starts with \`beast2\_\` and has extension
\`.xml\`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

create_temp_input_filename()
#> [1] "/github/home/.cache/beastier/beast2_70e1cf5c3be.xml"

check_empty_beaustier_folders()
```
