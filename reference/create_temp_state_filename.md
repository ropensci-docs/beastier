# Create a temporary file for the BEAST2 XML output file that stores its state.

Create a temporary file for the BEAST2 XML output file that stores its
state.

## Usage

``` r
create_temp_state_filename()
```

## Value

a temporary filename, that starts with \`beast2\_\` and has extension
\`.xml.state\`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

create_temp_state_filename()
#> [1] "/github/home/.cache/beastier/beast2_70e3d888bd6.xml.state"

check_empty_beaustier_folders()
```
